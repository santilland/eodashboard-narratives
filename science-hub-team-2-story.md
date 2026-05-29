---
cover-image: https://climate.esa.int/media/images/Ocean-Colour-CCI_.2e16d0ba.fill-600x314-c100.format-jpeg.jpg
date: 2025-01-01
theme: oceans
tags: ocean,water-quality,clustering,mediterranean
offifial: false
---

# Clustering Ocean Water Types Using Spectral EO Data <!--{ as="img" mode="hero" src="https://climate.esa.int/media/images/Ocean-Colour-CCI_.2e16d0ba.fill-600x314-c100.format-jpeg.jpg" }-->
### Authors: Enrico Biscaro¹, William Luty², Katie Lowery³ <!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->
> ¹ Ca’ Foscari University of Venice
² National Oceanography Centre
³ British Antarctic Survey


# 
*This story is based on results from the [Science Hub Challenges in September 2025](https://sciencehub.esa.int/2025/09/29/science-hub-challenges-september-2025/) organised and hosted by ESA's ESRIN, using multi-parameter satellite datasets (ocean color, sea surface temperature, sea level, and wind observations) combined with unsupervised machine learning clustering techniques to classify ocean water types, by students from the following organizations:*


## <!--{ nav="false" }-->
<p align="center">
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/cafoscari.png" alt="Ca' Foscari" height="80" style="margin: 0 15px;"/>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/noc-logo-full-colour.png" alt="NOC" height="80" style="margin: 0 15px;"/>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/bas-full-logo.png" alt="BAS" height="80" style="margin: 0 15px;"/>
</p>

## Challenge

Ocean water types - such as coastal, upwelling, oligotrophic, inland, and eutrophic waters - exhibit **distinct reflectance spectra and bio-optical/biogeochemical characteristics** ([Bi et al., 2024](https://doi.org/10.1002/lno.12606)) that reflect different ecological conditions and biological productivity ([Cui et al., 2020](https://doi.org/10.1016/j.isprsjprs.2020.02.017); [Uudeberg et al., 2020](https://doi.org/10.3390/rs12060931)) features which allows for the distinguishing and grouping different water types. These classifications are fundamental for **understanding marine ecosystems**, **monitoring water quality**, **assessing fisheries health**, **supporting climate research** while unraveling the compelex mechanisms controlling ocean biology, chemistry, and physics. 

Traditional methods for classifying ocean water types rely on **in-situ measurements** (e.g. diffuse attenuation coefficient, water inherent optical properties, and chlorophyll-a concentration) or **supervised classification** requiring extensive labeled training data. However, the spectral signatures captured by satellite sensors contain rich information that can be extensively and easily used to identify natural groupings in ocean properties. **Unsupervised learning approaches**, particularly clustering algorithms, offer a powerful way to discover these patterns directly from Earth observation data without predefined labels.

<div style="text-align: center;">
  <img 
    src="https://ars.els-cdn.com/content/image/1-s2.0-S003442572200339X-gr9_lrg.jpg" 
    width="450"
  /><br>
  <p>
    <b>Figure 1.</b> Satellite-derived water classes in the northwest Pacific region (VIIRS-SNPP snapshot; February 9, 2016; 750 m resolution). 
    The water classes and bio-optical data were extracted along the transect indicated by solid pink circles. 
    The square area delimited by the white dashed box is the region for extracting monthly time series data. 
    Black pixels represent invalid ocean color measurements 
    (<a href="https://doi.org/10.1016/j.rse.2022.113233" target="_blank">Wei et al., 2022</a>)
  </p>
</div>

This challenge leverages multiple Earth observation datasets including ocean color (chlorophyll-a concentration), sea surface temperature, sea level height anomalies, and atmospheric wind patterns to identify and map distinct water types based on their combined physical and biological properties.

## Objective

The primary objectives of this study are to:

1. **Apply unsupervised clustering algorithms** to classify ocean water types using multi-parameter Earth observation data.  
2. **Integrate spectral bands and derived biophysical indices** to effectively capture the multi-dimensional nature of ocean properties.  
3. **Validate identified clusters** against established oceanographic features and known water type classifications.  
4. **Generate comprehensive spatial and temporal maps** of water types across the Mediterranean Sea.  
5. **Analyze seasonal variations** in the distribution and characteristics of water types.

#### Overall Aim
This research aims to demonstrate how **machine learning** can uncover meaningful ecological patterns from **satellite-derived data**, thereby advancing both **operational oceanography** and **marine ecosystem management**.

## Use case <!--{ as="eox-map" mode="tour" }-->

### <!--{ layers='[{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"}},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"}},{"type":"Tile","properties":{"id":"cloudless-2024;:;EPSG:3857","title":"EOxCloudless 2024"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2024_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"}}]},{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857"}}]}]' zoom="5.5" center=[18.0,38.0] projection="" animationOptions={duration:500}}-->
#### Mediterranean Sea
The Mediterranean Sea represents an exceptional natural laboratory for the study and classification of ocean water types, owing to its **ecological significance** and **considerable economic value**. This semi-enclosed basin is characterized by a high degree of oceanographic complexity, shaped by the interplay of regional climate variability, diverse coastal processes, and intricate basin-scale circulation patterns. Its unique combination of environmental factors makes the Mediterranean an ideal setting for understanding the spatial and temporal variability of water properties and for advancing oceanographic research.

<div style="text-align: center;"> <img src="
https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/Globe2_mediterranee.png" width="600"/> <p><b>Figure 2.</b> The Mediterranean Sea.</p> </div>



**Key motivations for studying the Mediterranean:**

**Fisheries and Biodiversity Management**: Optimizing fish harvesting while preserving fish populations and marine biodiversity requires understanding the distribution and dynamics of different water types that support various marine habitats and food webs.

**Climate Change Monitoring**: Tracking physico-chemical parameters of Mediterranean waters in a changing climate is crucial, particularly considering the basin's contribution to the Atlantic Meridional Overturning Circulation (AMOC) and its sensitivity to warming trends.


## Data and Methods

#### Dataset
All variables were sourced exclusively from Copernicus Marine Service Level-4 (L4) products, meaning they consist of multi-sensor, gap-filled, optimally interpolated satellite datasets rather than model outputs or reanalyses. All layers therefore represent gridded EO-derived fields with full spatial coverage. 

The spatial resolution of the datasets ranges from approximately 0.04° to 0.1° (4–10 km) depending on the product.


| Category | Parameter ID | Description |
|:-:|:-:|:-:|
| 🌱 **Biological / Optical** | Chlorophyll-a concentration | Proxy for phytoplankton biomass and primary productivity; derived from ocean color sensors |
| 🌡️ **Physical** | Sea Surface Temperature (SST) | Indicator of water mass characteristics and thermal structure |
|  | Sea Level Height Anomaly | Reflects ocean circulation patterns and eddy activity |
| 🌬️ **Atmospheric Forcing** | Eastward wind component (U-wind) | Represents zonal atmospheric forcing |
|  | Northward wind component (V-wind) | Represents meridional atmospheric forcing and wind stress effects |




<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/fig4.png" 
        style="max-width: 100%; width: 1300px; height: auto;"
        alt="Multi-parameter dataset"
    />
    <p style="text-align: center; margin-top: 10px;">
        <b>Figure 4.</b> Example data layers: chlorophyll-a concentration, sea surface temperature, sea level height anomaly, and wind components used in the clustering analysis
    </p>
</div>

#### Methodology workflow

**1. Data Acquisition and Preprocessing**
- Downloaded monthly time series of all parameters for the Mediterranean Sea region
- Ensured spatial and temporal alignment across all datasets
- Handled missing values and quality control flags

**2. Feature Engineering**
- Combined biological, physical, and atmospheric variables into a multi-dimensional feature space
- Normalized all variables to comparable scales to prevent dominance by parameters with larger absolute values
- Created composite monthly datasets integrating all five parameters

**3. Cluster Number Selection**
- Applied the elbow method to determine optimal number of clusters
- Calculated inertia error (within-cluster sum of squares) for different cluster numbers
- **Elbow analysis suggested 5 clusters as optimal** based on inertia curve inflection

**4. K-means Clustering Application**
- Applied K-means algorithm with k=8 clusters
- Used multiple random initializations to ensure robust convergence
- Assigned each pixel to its nearest cluster centroid in the multi-dimensional feature space

**5. Cluster Characterization**
- Analyzed mean values of each parameter within identified clusters
- Interpreted clusters in terms of oceanographic water types (eutrophic, oligotrophic, coastal)
- Examined spatial distribution patterns and geographic coherence
- Steps 4 (clustering) and 5 (cluster evaluation and selection of k) were performed in parallel: firstly by testing many k-values with K-means, then chosing the number of clusters that produced meaningful spatial patterns.


**6. Temporal Analysis**
- Tracked seasonal evolution of cluster distributions
- Identified stable versus dynamic water type regions
- Analyzed transitions between water types through the annual cycle

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/team2_method.png" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Analysis workflow"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 5.</b> Analysis workflow from multi-parameter data acquisition through clustering to water type characterization.
    </p>
</div>

## Results

#### Water Type Identification

The clustering analysis successfully identified three primary ocean water types from the eight clusters tested, with distinct biogeochemical and physical characteristics. To note that, cluster types were not assigned a priori; instead, each cluster was interpreted by examining its mean SST, chlorophyll-a, wind components, and SSH, alongside its spatial footprint. Cluster interpretations were based on the **statistical properties of each cluster**.

**Cluster 1 - Eutrophic Water**:
- Characterized by **colder waters** relative to basin average
- Associated with **eastward winds** driving coastal upwelling
- **Medium chlorophyll-a content** (1-3 mg/m³) indicating elevated productivity
- Typically found in upwelling zones and areas of nutrient enrichment

**Cluster 2 - Coastal Water**:
- Distinguished by **very high chlorophyll-a concentrations** (>3 mg/m³)
- Elevated **sea surface height** in coastal boundary regions
- Represents nutrient-rich waters influenced by terrestrial runoff and coastal processes
- Most productive water type supporting high biological activity

**Cluster 7 - Oligotrophic Water**:
- Dominated by **warmer waters** characteristic of stratified conditions
- Associated with **northward wind and wind stress** patterns
- **Low chlorophyll-a content** (<0.3 mg/m³) indicating nutrient limitation
- Represents the ultra-oligotrophic central Mediterranean basins

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/fig5.png" 
        style="max-width: 100%; width: 1000px; height: auto;"
        alt="Cluster characteristics"
    />
    <p style="text-align: center; margin-top: 10px;">
        <b>Figure 6.</b> Characteristics of the three main water type clusters showing distributions of chlorophyll-a, SST, and wind patterns
    </p>
</div>

Regarding the **cluster differences**, these represent the pixel-wise change in assigned cluster between January and August. For example, red regions indicate pixels classified as Cluster 1 in January but as Cluster 7 in August. Blue regions show the opposite transition.

Despite using 8 clusters, the algorithm effectively utilized only 3 distinct clusters, with the remaining clusters either rarely assigned or representing transitional states. This suggests that Mediterranean water types can be meaningfully described by three primary categories, though finer divisions may be needed for specific applications.


#### Spatial Distribution

The spatial distribution of identified water types shows strong geographic coherence aligned with known Mediterranean oceanography:

- **Coastal waters (Cluster 2)** dominate near coastlines, particularly in the Northern Adriatic, Gulf of Lions, and along the North African coast
- **Oligotrophic waters (Cluster 7)** occupy the central basins, especially the eastern Mediterranean
- **Eutrophic waters (Cluster 1)** appear in transitional zones and areas influenced by upwelling or mixing processes

These interpretations are consistent with previous Mediterranean water-type studies (e.g., Volpe et al., 2019; Uudeberg et al., 2020), although no formal quantitative comparison was performed.



#### Seasonal Variations
Seasonal patterns were analyzed to track cluster evolution. Analysis of the seasonal cycle reveals temporal dynamics in water type distribution:

- **Oligotrophic waters (Cluster 7)** show expansion during summer months when stratification is strongest, then contract in winter
- **Eutrophic waters (Cluster 1)** exhibit seasonal variability linked to wind-driven mixing and upwelling events
- **Coastal waters (Cluster 2)** remain relatively stable throughout the year, though this may represent a limitation requiring further investigation. Cluster 2 shows no seasonal change because the coastline does not shift seasonally, reinforcing its identification as a coastal water class.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/SeasonalClusters_percentage-change.png" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Seasonal cycle of clusters"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 7.</b> Seasonal evolution of water type clusters showing expansion and contraction of oligotrophic and eutrophic waters through the annual cycle. Percentage change refers to the relative change in cluster area for each season compared to summer. 
    </p>
</div>

The seasonal patterns align with known Mediterranean dynamics: winter mixing enriches surface nutrients leading to spring blooms (eutrophic expansion), followed by summer stratification that extends oligotrophic conditions and reduces productivity in open waters.





<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-2/fig6.png" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Seasonal cycle of clusters"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 8.</b> Seasonal evolution of water type clusters showing expansion and contraction of oligotrophic and eutrophic waters through the annual cycle.
    </p>
</div>





## Conclusions

This study demonstrates the effectiveness of unsupervised clustering for identifying and mapping ocean water types from multi-parameter satellite observations. The multi-variable approach (Chl-a + SST + SSH + winds) was critical for distinguishing water types. Tests using subsets of variables (e.g., only Chl-a + SST) resulted in fewer or less stable clusters, typically merging oligotrophic and eutrophic waters.  
SSH and wind components helped isolate dynamical conditions such as upwelling, which improved separation between eutrophic and transitional water masses. While not quantified formally, sensitivity tests showed that removing physical variables reduced ecological interpretability of the clusters.

Key findings of this study include:

1. **Three distinct water types identified**: Coastal (high productivity), eutrophic (moderate productivity), and oligotrophic (low productivity) waters distinguished by combined biological, physical, and atmospheric characteristics

2. **Geographic coherence**: Spatial patterns align with known Mediterranean oceanography, validating the clustering approach against established understanding

3. **Seasonal dynamics captured**: Temporal analysis reveals expansion/contraction of water types consistent with seasonal stratification and mixing cycles

4. **Multi-parameter synergy**: Integration of chlorophyll-a, SST, sea level height, and wind components provides richer characterization than single-parameter approaches

**Practical applications** include:
- Supporting marine spatial planning and fisheries management by mapping productive zones
- Monitoring ecosystem shifts under climate change scenarios
- Validating biogeochemical models with observationally-derived water type classifications
- Identifying optimal locations for aquaculture or marine protected areas

**Study limitations and future directions:**

1. **Cluster number selection**: Statistical optimum (5 clusters) provided insufficient detail, while chosen number (8) resulted in only 3 active clusters—suggesting need for adaptive cluster selection methods

2. **Coastal water stability**: Lack of seasonal variation in Cluster 2 (coastal waters) may indicate need for higher temporal resolution or separate coastal-specific analysis

3. **Validation needed**: No quantitative validation against in-situ measurements or existing water type classifications was performed

4. **Algorithm exploration**: Testing alternative clustering methods (hierarchical, DBSCAN, Gaussian mixture models) could improve classification

5. **Additional parameters**: Including sea surface salinity, turbidity, or fluorescence line height could enhance water type discrimination

**Future work priorities:**
- Extend analysis to other ocean basins for method generalization
- Incorporate in-situ validation data from research cruises and Argo floats
- Develop operational products for near-real-time water type mapping
- Investigate machine learning approaches for temporal prediction of water type transitions

The framework established here provides a foundation for automated ocean water type classification from Earth observation data, with potential applications in operational oceanography, ecosystem monitoring, and climate change impact assessment.

## <!--{ as="div" }--> Open Science

| **Name**                                                                                                                                       | **Type**            | **Agency / Provider**                     | **Description / Usage**                                                                                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **[Mediterranean Ocean Colour Product](https://doi.org/10.5194/os-15-127-2019)**                                        | Dataset             | CNR-ISAC / ESA               | Operational multi-sensor Level 3 chlorophyll-a concentration product providing monthly composites of phytoplankton biomass across the Mediterranean Sea.                            |
| **[Mediterranean SST Optimally Interpolated Dataset](https://doi.org/10.1016/j.rse.2016.01.019)**                                                                                       | Dataset | CNR-ISAC                        | AVHRR Pathfinder sea surface temperature data (1982-2012) extended with recent observations, providing high-quality thermal structure information.                                     |
| **[Multi-dimensional Sea Surface Salinity](https://doi.org/10.1016/j.rse.2016.07.033)**                                          | Dataset     | CNR-ISAC               | Integrated SMOS satellite and in-situ salinity observations providing water mass characteristics (not used in current study but relevant for future work).                                                     |
| **[Mediterranean Sea Level Anomaly](https://resources.marine.copernicus.eu/)**                          | Dataset | Copernicus Marine Service | Altimetry-derived sea level height anomalies indicating ocean circulation and eddy activity.                                               |
| **[ERA5 Wind Components](https://www.ecmwf.int/en/forecasts/datasets/reanalysis-datasets/era5)**                          | Dataset | ECMWF | Reanalysis-derived eastward (U) and northward (V) wind components at 10m height for atmospheric forcing characterization.                                               |

#### Notebook
Access the complete analysis notebook to reproduce the clustering workflow. This notebook has been developed and validated on the [DeepESDL environment](https://earthsystemdatalab.net/), where the necessary data, tools, and execution kernels are available. DeepESDL is part of ESA's [EarthCODE initiative](https://earthcode.esa.int/), enabling open and reproducible Earth Science. Sponsored access can be requested through ESA's [Network of Resources](https://nor-discover.org/).
<iframe width="100%" height="600" src="https://esa-eodashboards.github.io/eodashboard-notebooks/notebooks/oceanographic-patterns-clustering/" frameborder="0"></iframe>


#### References

- Berthon, J.-F., and Zibordi, G. (2004). Bio-optical relationships for the northern Adriatic Sea. *International Journal of Remote Sensing*, 25, 1527-1532.

- Buongiorno Nardelli, B., Droghei, R., and Santoleri, R. (2016). Multi-dimensional interpolation of SMOS sea surface salinity with surface temperature and in situ salinity data. *Remote Sensing of Environment*, 180, 392-402.

- Droghei, R., Buongiorno Nardelli, B., and Santoleri, R. (2016). Combining in-situ and satellite observations to retrieve salinity and density at the ocean surface. *Journal of Atmospheric and Oceanic Technology*, 33, 1211-1223.

- Embury, O., Merchant, C.J., Good, S.A., et al. (2024). Satellite-based time-series of sea-surface temperature since 1980 for climate applications. *Scientific Data*, 11, 326.

- Pisano, A., Nardelli, B.B., Tronconi, C., and Santoleri, R. (2016). The new Mediterranean optimally interpolated pathfinder AVHRR SST Dataset (1982–2012). *Remote Sensing of Environment*, 176, 107-116.

- Sammartino, M., Aronica, S., Santoleri, R., and Buongiorno Nardelli, B. (2022). Retrieving Mediterranean Sea Surface Salinity Distribution and Interannual Trends from Multi-Sensor Satellite and In Situ Data. *Remote Sensing*, 14, 250.

- Volpe, G., Buongiorno Nardelli, B., Colella, S., et al. (2018). An Operational Interpolated Ocean Colour Product in the Mediterranean Sea. In *New Frontiers in Operational Oceanography*, edited by E.P. Chassignet et al., pp. 227–244.

- Volpe, G., Colella, S., Brando, V.E., et al. (2019). Mediterranean ocean colour Level 3 operational multi-sensor processing. *Ocean Science*, 15(1), 127-146.

