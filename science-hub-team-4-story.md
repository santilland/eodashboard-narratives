---
cover-image: https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2022/10/svalbard/24544693-1-eng-GB/Svalbard_pillars.jpg
date: 2025-05-20
theme: cryosphere
tags: sentinel-1, C-band, machine learning, Arctic, Svalbard, Remote Sensing
official: false

---

# Wet snow mapping with multimodal foundation models - can we drop the reference?  <!--{ as="img" mode="hero" src="https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2022/10/svalbard/24544693-1-eng-GB/Svalbard_pillars.jpg" }-->
### Authors: Leam Howe¹, Sean Ó Héir¹, Miguel Espinosa Minano¹ <!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->
1 - University of Edinburgh

# 
*This story is based on results from the [Science Hub Challenges in September 2025](https://sciencehub.esa.int/2025/09/29/science-hub-challenges-september-2025/) organised and hosted by ESA's ESRIN, using [Sentinel‑1 satellite](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Sentinel-1) data and Geospatial Foundation Models (GFMs) for snow classification, by students from the Universty of Edinburgh:*

##  <!--{ nav="false"}-->
<p align="center">
  <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/download.png?raw=true" 
       alt="University of Edinburgh" 
       height="80"/>
</p>




## Challenge
Snow varies greatly in its characteristics and radiative effects. Keen skiers are likely familiar with variations in snow wetness. Two primary types are dry snow and wet snow, which differ in water content, density, grain size, and formation conditions. Dry snow is powdery and light, occurring in cold temperatures well below freezing, whereas wet snow contains higher water content, is denser, and forms near or above freezing temperatures.

#### Why map it?
Mapping wet snow is not just about skiing conditions; it is a critical variable for predicting flood risks from "Rain-on-Snow" events and forecasting wet slab avalanches. Beyond hazards, accurate detection monitors ecological threats—such as the formation of basal ice that locks away winter grazing for Arctic wildlife—and signals the onset of seasonal runoff for hydropower management. 

Mapping of wet snow at a large-scale is only possible using radar remote sensing because radar can penetrate the surface and provide insight into the internal structure of the snow, whereas optical imagery only provides information from the surface. Historically, passive microwave radiometers (including the AMSR series) have been widely used for large-scale snowmelt detection, thanks to the strong contrast in microwave emissivity between dry and wet snow. While these sensors offer daily global coverage, their coarse spatial resolution (25–50 km) limits their utility for regional and catchment-scale applications. Thermal infrared observations, can offer complementary surface-temperature information at a moderate resolution (~500 m) that is particularly relevant for detecting the onset of surface melt. However, high-resolution wet snow mapping is only possible using synthetic aperture radar (SAR), such as the ESA Sentinel-1 C-band satellite sensor.

Large-scale wet snow mapping from Earth Observation instruments , remains challenging due to the complex interaction of radar signals with snow characteristics.
C-band radar can penetrate the surface of snow and provide insight into the internal structure.

Traditionally, wet snow is identified in SAR data by the difference in penetration depth between wet and dry snow.  Dry snow allows deeper penetration of C-band radar signals (up to 10 meters), wet snow’s higher liquid water content absorbs microwave radiation, limiting penetration to less than 10 centimeters (as shown in figure 1). This leads to a strong contrast in radar backscatter intensity, with wet snow showing significantly lower backscatter compared to dry snow and dry snow-free ground.



<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/image_sar_snow.png?raw=true" width="500"/> <p><b>Figure 1.</b>Figure from Carlo Marin et al. 2020 (https://tc.copernicus.org/articles/14/935/2020/), schematic representation of c-band microwave interaction with wet and dry snow. C-band microwaves can penetrate through 10 m of dry snow vs ~10 cm of wet due to the high dielectric loss caused by liquid water. </p> 

</div>
  
However, wet-snow mapping with SAR is often confused by wet soil/vegetation because liquid water in the snowpack and wet ground can give similar backscatter signatures. Operational workflows therefore commonly require a summer/dry reference image (or a clear optical image close to the date) to separate wet snow. This is achieved by calculating the backscatter difference between the active and reference images, typically applying a threshold of around -3dB to identify the expected [signal drop caused by melting snow](https://doi.org/10.1109/36.842004). This reliance on reference imagery is a significant limitation; finding a high-quality baseline is difficult, and the method assumes temporal stability in ground conditions, ignoring changes in vegetation or soil roughness that can lead to misclassification. 

#### Our idea

**Multimodal geospatial Foundation Models (GFMs)** offer a promising alternative by synthesising diverse Earth observation data into a unified representation. Here we wanted to test if the latent representations within a pre-trained GFM could be fine-tuned to enable single-pass wet snow mapping from SAR imagery alone—removing the need for a reference image.

To achieve this "reference-free" approach, the model must overcome the inherent physical ambiguities of single-pass SAR data. Traditional operational workflows rely on change detection, calculating the temporal difference in backscatter against a summer reference image to identify the characteristic signal drop caused by melting snow. However, this differencing method is highly vulnerable to false positives if ground conditions (such as soil moisture) change between acquisitions.

Our hypothesis explores replacing this temporal differencing with spatial context to resolve the single-pass ambiguity. In a single SAR image, wet snow, flooded soil, and wet vegetation all appear identically dark. However, they form very different spatial patterns on the landscape. The transition from dry snow to wet snow, for example, is dictated by temperature; it typically forms a distinct, continuous melt boundary (following the ~0°C isotherm) that tracks along an elevation gradient. We hypothesise that by fine-tuning a GFM on dual-polarisation (VV and VH) SAR patches, the algorithm can learn to recognise these structural boundaries. By evaluating these textures and spatial shapes rather than isolated pixel values, the model can learn to distinguish the contiguous edge of an active melt zone from the irregular pooling of flooded lowland soil or wet forests. 



<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/GFM.png?raw=true" width="500"/> <p><b>Figure 2.</b>Unified multimodal Earth foundation model. Large AI models trained on diverse airborne and satellite data integrate multiple sensor types to enable scalable, transferable, and few-/zero-shot learning for tasks such as land cover classification, flood detection, and forest monitoring. Figure from [DOFA paper](https://arxiv.org/abs/2403.15356)</p> 

</div>
  

## Objective

**Goal:** Evaluate if foundation-model embeddings can produce accurate, reference-free wet snow maps from one Sentinel-1 scene.This involved: 
* **Ingest**: Sentinel-1 C-band SAR data 
* **Fine-Tune**: fine-tuning a Geospatial Foundation Model to perform semantic segmentation of snow types, distinguishing wet snow, dry snow, and no snow.
* **Validate**: Predictions from the model were validated against an independent dataset, enabling assessment of classification accuracy against existing products and operational potential for snow mapping applications.

## Use case 
#### Svalbard
Svalbard, an Arctic archipelago, is an ideal testbed for wet snow mapping due to its extreme climate and diverse snow conditions. Accurate monitoring of wet snow here supports water resource management, flood risk assessment, and climate studies in this sensitive region. This region was also chosen because the Norwegian Meteorological Institute has made an [excellent dataset of SAR wet snow maps](https://adc.met.no/dataset/64a3bb5a-47d5-550b-ad8e-946cd03be8f0) of Svalbard openly available to use through the Arctic Data Centre; subsets of this dataset were used to train and validate the model used in this study. The idea being that once trained on this region the model could then be applied to other regions without a reference image being required and provide valuable insights for environmental monitoring and decision-making in other snow covered regions.


<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/Globe4_svalbard.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Use cases/forests locations"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 3.</b> Use case: the Svalbard archipelago.
    </p>
</div>




	
## Data and Methods
#### Dataset
* **Input data**: Sentinel-1 satellite dual imagery (VV and VH patches)
* **Labels**: NMI [dataset of SAR wet snow maps of Svalbard](https://adc.met.no/dataset/64a3bb5a-47d5-550b-ad8e-946cd03be8f0) at 100 m resolution with 4 classes (wet snow,  dry snow, no data, bare ground, and water). Dataset by [Vickers et al., 2022](https://doi.org/10.3389/feart.2022.868945). 
* **Classes/Output data**: Wet snow, dry snow, no data, bare ground, and water.
* **Coverage**: A subset of approximately 150 scenes were used this project


#### Methodology workflow
The approach builds on a Geospatial Foundational Model (GFM) that has been pre-trained on large-scale geospatial data. [PANGAEA-BENCH](https://arxiv.org/abs/2412.04204) is a framework for implementing and comparing GFMs developed by ESA Phi-Lab, so we thought this would be a good starting point. Our workflow consisted of the following steps:
* **Data preparation**: In the limited 2-day time-frame of this project, we only extracted a small subset of the Svalbard dataset composed of ~150 image patches. To match the input imagery with the coarse resolution of the labelled dataset, we resampled the Sentinel-1 data to 100 m. 
* **Model Initialization**: The [CROMA model](https://arxiv.org/abs/2311.00566) is used as the pretrained backbone (encoder) to extract meaningful geospatial features from Sentinel-1 input data.
* **Decoder Integration**: A UPerNet decoder is added to the pretrained encoder to enable pixel-wise classification, producing a snow segmentation map.
* **Fine-Tuning Process**: The model is fine-tuned using the small labeled dataset (~150 scenes). The encoder is partially frozen to retain foundational geospatial knowledge, while the decoder is trained for the specific segmentation task.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src=" https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/methods1.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt=""
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 4.</b> Schematic of input and output of the model. Input on the left is the Sentinel-1 VV and VH backscatter signals and from this we create a wet snow map by fine-tuning  a geospatial foundation model.
    </p>
</div>
	

## Results (preliminary
#### Accuracy metrics
* **Dry Snow**: Early tests showed high potential for dry snow detection (>90% accuracy in initial epochs).
* **Wet Snow Ambiguity**: The model struggled to differentiate wet snow from wet ground features, with IoU metrics stalling around 55–60%.


<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/figure5_updated.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Validation results"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 5.</b> Validation results.
    </p>
</div>


#### Visual interpretation
From the VV and VH backscatter images, clear textural differences can be observed (brighter and darker streaks) likely corresponding to variations in surface roughness, water, and snow conditions. Comparing the SAR images and the labels, it is very hard for the naked human eye to distinguish the wet snow from snow, therefore, the model will have to learn to pick up patterns from the subtle backscatter differences.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-4/results2.png?raw=true" style="max-width: 100%; width: 800px; height: auto;" alt="" /> <p style="text-align: center; font-size: 1.2em; margin-top: 10px;"> <b>Figure 6.</b> Comparison of input Sentinel-1 VV and VH images, predicted segmentation mask, and target mask. </p> </div>

* **Observations**: While the model identified broad homogeneous zones like open water (see figure 6), it failed to capture the subtle textural differences in transitional zones.
* **Interpretation**: The decision to downsample Sentinel-1 to 100 m likely resulted in substantial information loss. By averaging out the fine-scale backscatter textures inherent in high-res SAR data, we removed the very cues the model needed to distinguish complex surfaces. The results are likely negatively impacted due to the small sample size and lack of topographical context and look-angle in the input channels.


## Conclusions
* **Summary**: This project represents a **quick "first look" feasibility test** conducted over a 2-day challenge period. Due to the small dataset (~150 scenes) and time constraints, **current results are inconclusive**. The model in its current state cannot yet reliably distinguish wet snow from wet soil without a reference.
However, the experiment highlighted specific technical barriers that, if addressed, could unlock success.

####  Future Roadmap: Data
* **Native Resolution**: Stop downsampling. Future iterations must use Sentinel-1 at its native resolution (approx. 10–20 m) to preserve textural information.
* **Scale Up**: Process and ingest the full Sentinel-1 Svalbard wet snow dataset (Vickers et al., 2022), rather than a small subset. The 2-day constraint limited us to a fraction of the available data; a larger dataset can be essential for machine learning models to learn complex and nuanced features.
* **Local Incidence Angle (LIA**): Add LIA as an additional input channel. Radar backscatter is heavily dependent on the angle of interaction, and this missing context likely confused the model.
* **Topography**: Integrate Digital Elevation Models (DEM) to help the model rule out wet snow in low-lying, warm valleys where wet soil is more likely.
* **Augmentation**: Implement robust data augmentation (rotation, flipping) to prevent overfitting.
* **Complementary Data Sources**: Integrate thermal infrared observations (e.g., GCOM-C/SGLI) and passive microwave data (e.g., AMSR2) as additional input channels, to provide surface temperature and snowmelt-state context that could help the model better separate wet snow from wet soil signatures.

#### Future Roadmap: Model Architecture
* **Encoders**: Test different backbone architectures to see which pre-trained weights offer the best transfer learning for polar environments.
* **Decoders**: Experiment with different segmentation heads beyond UPerNet.
* **Loss Functions**: Explore loss functions that penalize boundary errors more heavily to sharpen the detection of snow-lines.



## <!--{ as="div" }--> Open Science
| **Name**                                                                                                                                       | **Type**            | **Agency / Provider**                     | **Description / Usage**                                                                                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **[Sentinel-1 Snow Classification Dataset](https://sentinel.esa.int/web/sentinel/missions/sentinel-1)**                                        | Dataset             | ESA (European Space Agency)               | A small dataset (~150 images) of Sentinel-1 VV and VH polarization patches used to train a segmentation model for snow classification. Classes include wet snow, dry snow, bare ground, water, and no data.                            |
| **[PANGAEA-BENCH Framework](https://arxiv.org/abs/2412.04204)**                                                                                       | Framework / Toolkit | PANGAEA Consortium                        | Used to fine-tune geospatial foundational models (GFMs) for Earth observation tasks. Enabled the training of the decoder (UPerNet) on the pre-trained CROMA encoder for the snow segmentation task.                                     |
| **[CROMA Geospatial Foundational Model](https://www.esa.int/Applications/Observing_the_Earth/CROMA)**                                          | Model / Encoder     | CROMA               | Pre-trained encoder providing general geospatial representations. Used as the backbone model, fine-tuned with a UPerNet decoder to produce pixel-wise snow classification outputs.                                                     |
| **[EO Dashboard](https://eodashboard.org/explore/?x=15.0000&y=48.0000&z=4.0000&datetime=2025-09-19&template=expert)**                          | Platform / Web Tool | EO Dashboard Consortium (ESA, NASA, JAXA) | Provides base layers and visualization tools for interactive exploration of NDVI and other Earth observation indicators, potentially useful for validating and visualizing model outputs.                                               |




#### References
- PANGAEA: A Global and Inclusive Benchmark for Geospatial Foundation Models [Access paper](https://arxiv.org/abs/2412.04204).
- CROMA Geospatial Foundational Model. [Access paper](https://arxiv.org/abs/2311.00566).
- Carlo Marin et al., 2020.[Access paper](https://tc.copernicus.org/articles/14/935/2020/).
-  Vickers et al., 2022. [Access paper](https://doi.org/10.3389/feart.2022.868945). 






