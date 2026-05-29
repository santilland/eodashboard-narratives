---
cover-image: https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-5/Tajikistan_wikivoyage_banner.jpg
date: 2025-01-01
theme: cryosphere
tags: glaciers,climate,third-pole, sentinel-1
official: false

---

# Glacier monitoring under global warming trends through remote sensing – An example from The Third Pole  <!--{ as="img" mode="hero" src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/main/stories/ScienceHub-Challenge-September-2025/Team-5/Tajikistan_wikivoyage_banner.jpg" }-->
### Authors: Sheharyar Ahmad¹, Federico Scoto¹, Ginevra Chelli¹, Arslaan Akhtar¹ <!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->
> ¹ Ca’ Foscari University of Venice

# 
*This story is based on results from the [Science Hub Challenges in September 2025](https://sciencehub.esa.int/2025/09/29/science-hub-challenges-september-2025/) organised and hosted by ESA's ESRIN. The challenge focused on monitoring properties of snow, glaciers and sea ice using the [DeepESDL platform](https://earthsystemdatalab.net/). It was developed by a team from Ca’ Foscari University of Venice.*

##  <!--{ nav="false"}-->

<p align="center">
  <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/cafoscari.png?raw=true" 
       alt="University of Edinburgh" 
       height="80"/>
</p>


## Challenge
The Third Pole region, encompassing the Hindu Kush-Karakoram-Himalaya mountain ranges, contains the largest concentration of glaciers outside the polar regions. These glaciers are critical water sources for over two billion people in Asia. However, understanding glacier dynamics in this region is complicated by the **"Karakoram anomaly"**, a phenomenon where some glaciers show *stability or even slight growth* despite global warming trends. Monitoring glacier properties such as surface temperature, mass balance, and supraglacial lake formation is essential for water resource management, understanding climate impacts, and predicting flood risks. Traditional field measurements are challenging in these remote, high-altitude environments, making satellite remote sensing the primary tool for comprehensive glacier monitoring.

<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/figure1_team5.png?raw=true" /> <p><b>Figure 1.</b> Conceptual diagram showing the key components of glacier monitoring: surface temperature variations, mass balance changes, and the formation of supraglacial lakes in response to climate forcing.</p> 

</div>

The challenge addresses a specific scientific question: **How can cooler summers coincide with higher water availability in the western Pamir region?** 
Glacier melt is the primary source of freshwater for communities downstream in this region. Melt typically peaks during warm summer months, so a trend of cooling summer temperatures would be expected to reduce water availability, yet observations suggest the opposite, pointing to a more complex dynamic driven by seasonal shifts in melting patterns. 
This paradox requires integrating multiple remote sensing datasets to understand the complex interaction between seasonal temperature patterns, glacier mass balance, and water storage dynamics.

## Objective

The objective of this study was to investigate the Kekesayi Glacier in the Pamir Mountains to understand its anomalous behavior under climate change. Specifically, the study aimed to:

- Analyze seasonal and annual Land Surface Temperature (LST) trends over the glacier from 2002 to 2018
- Detect and quantify changes in supraglacial lake area as a proxy for water availability
- Map moisture extent across the glacier surface to assess mass balance changes
- Integrate multi-sensor observations to explain the apparent paradox of warming winters, cooling summers, and increased water availability

This integrated approach enables a comprehensive understanding of glacier dynamics that goes beyond simple temperature or area change assessments.

## Use case <!--{ as="eox-map" mode="tour" }-->

### <!--{ layers='[{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"}},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"}},{"type":"Tile","properties":{"id":"cloudless-2024;:;EPSG:3857","title":"EOxCloudless 2024"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2024_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"}}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"MODIS_LST_Pamir;:;2d96aa0d-5170-4979-b00e-e9e3eb1d3308;:;MODIS_LST_Pamir;:;EPSG:3857","title":"MODIS Land Surface Temperature"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["MODIS_LST"],"TILED":true,"TIME":"2015-09-01T00:00:00Z/2015-09-30T23:59:59Z"}}}]},{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857"}}]}]' zoom="11.5" center=[75.1,38.3] projection="" animationOptions={duration:500}}-->
#### Kekesayi Glacier, Pamir Mountains
The Kekesayi Glacier is the largest glacier in the Muztagh Ata area of the Pamir Mountains, located at the junction of several major Asian mountain systems. This heavily debris-covered glacier shows no significant frontal change despite regional climate warming, making it an ideal case study for understanding the Karakoram anomaly.

The Pamir Mountains, often called the "Roof of the World," are situated in Central Asia at the intersection of the Himalayas, Tian Shan, Karakoram, Kunlun, and Hindu Kush ranges. The region experiences marked interannual variability in temperature and precipitation, creating complex glacier dynamics.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/Globe5_Pamir.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Kekesayi Glacier location"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 2.</b> Location of Kekesayi Glacier in the Pamir Mountains, Central Asia.
    </p>
</div>

## Data and Methods
#### Dataset
The study integrated three primary satellite datasets:

- **MODIS AQUA L3C Daily LST Data Cube (CCI)**: 1km spatial resolution, 2002–2018 time range, providing daytime Land Surface Temperature measurements
- **Sentinel-2 (S2L2A)**: 10m spatial resolution, three time points (2015, 2017, 2020), used for supraglacial lake detection as a proxy for water availability
- **Sentinel-1 GRD**: 10m spatial resolution, three time points (2015, 2017, 2020), used for moisture extent and mass balance assessment

Temperature trend analysis was supplemented with ECMWF ERA5 reanalysis data to provide climatic context, showing marked interannual variability with higher temperature anomalies in winter since the 1980s and slightly positive Surface Mass Balance (SMB).

#### Methodology workflow

**1. Land Surface Temperature Analysis (MODIS L3C)**
<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/team5_method1.png?raw=true" /> <p><b>Figure 3.</b> Annual & Seasonal Mean LST ove Kekesayi Glacier.</p> </div>


**2. Supraglacial Lake Detection (Sentinel-2)**
<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/team5_method2.png?raw=true" /> <p><b>Figure 4.</b> Glacier lake area change detection.</p> </div>


**3. Moisture Extent Mapping (Sentinel-1)**
<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/team5_method3.png?raw=true" /> <p><b>Figure 5.</b> Moisture extent over the Kekesayi glacier.</p> </div>


## Results 


#### Seasonal Land Surface Temperature Patterns (MODIS L3C)
Maps of seasonal LST averaged over 2002-2018 reveal marked spatial variability between different areas of the Kekesayi Glacier, particularly between accumulation and ablation zones. As expected, during autumn and spring seasons, LST is higher in the ablation zone compared to the accumulation zone. 

**The most striking finding concerns the seasonal trend behaviour rather than the absolute spatial pattern**. While the ablation zone appears colder than surrounding terrain in summer, this cooling effect is not unique to summer and can be partly explained by well-known glacier processes such as debris-insulated ice surfaces and katabatic winds transporting cold air from the accumulation zone downslope. Similar contrasts between glacier surfaces and surrounding bedrock are visible in spring and autumn.

Therefore, the key signal does not lie in the spatial temperature contrast itself, but in the seasonal trends over time. Despite global warming, summer LST over the ablation zone does not show a significant warming trend, whereas winter exhibits a pronounced warming tendency. This seasonal asymmetry is consistent with previous studies (e.g., Li et al., 2023) suggesting that enhanced winter warming and precipitation, rather than increased summer melt, are major contributors to the Karakoram anomaly.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/results_team5.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Kekesayi Glacier location"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 6.</b> Land surface temperatures (LST)
    </p>
</div>


#### Temperature Trend Analysis
We analysed LST time series trend by quantifying pixels inside the ablation zone of glacier for linear trend estimation. A significant warming trend (R²= 0.56) is observed in winter, while autumn and spring show a cooling trend (R² 0.34 and 0.43, respectively). Notably during Summer a non significant cooling trend (R² = 0.05) can be also observed.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/results2_team5.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Kekesayi Glacier location"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 7.</b> Seasonal Land Surface Temperature (LST) trends over the ablation zone of Kekesayi Glacier (2002–2018), expressed in degrees Celsius (°C). Arrows indicate the direction of the linear trend for each season: upward arrows denote warming and downward arrows denote cooling. The glacier outline is shown in blue, with the shaded area indicating the ablation zone where pixel-level trend analysis was performed. Winter shows a statistically significant warming trend (R² = 0.56), while autumn and spring show cooling trends (R² = 0.34 and 0.43, respectively). Summer shows a non-significant cooling trend (R² = 0.05).
    </p>
</div>



<!--no-nav=true -->  
## Supraglacial Lake Expansion (Sentinel-2)
Sentinel-2 analysis using NDWI (threshold ≥ 0.11) to detect water pixels revealed substantial growth in supraglacial lake area:

- **September 2015**: 0.16 km²
- **September 2020**: 0.406 km²

This represents a **154% increase** in lake area over five years, indicating enhanced water availability despite cooler summer temperatures. The expansion likely reflects a combination of increased meltwater availability and evolving glacier drainage dynamics. While warmer winters may enhance meltwater production and storage, supraglacial lake formation is also strongly controlled by surface topography and the efficiency of englacial and subglacial drainage pathways. Variability in channel closure or blockage can significantly influence lake extent, even without major changes in meltwater supply.

Therefore, supraglacial lake expansion should be interpreted as an integrated signal of meltwater production and drainage system evolution, rather than as a direct proxy for increased winter melt alone.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/results3_team5.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Supraglacial lake comparison"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 8.</b> Comparison of supraglacial lakes between September 2015 (left) and September 2020 (right), showing significant expansion in lake area.
    </p>
</div>

## Moisture Extent Evolution (Sentinel-1)
Sentinel-1 moisture mapping at the end of summer season shows a dramatic increase in surface moisture extent:

- **September 2015**: 2.54 km²
- **September 2017**: 3.34 km²
- **September 2020**: 8.2 km²

The moisture extent maps generally coincide with supraglacial lake locations but cover a larger area, indicating subsurface water storage and saturated debris cover. The **223% increase** from 2015 to 2020 demonstrates substantial changes in glacier hydrology.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-5/results4_team5.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Moisture extent evolution"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 9.</b> Evolution of moisture extent across Kekesayi Glacier from 2015 to 2020, showing progressive increase in wet areas.
    </p>
</div>

Wet snow (moisture extent) was identified using a method that looks at changes in backscatter. The reference for dry snow was defined as the average σ⁰ during the winter when conditions are frozen. Pixels that showed a decrease greater than −2 dB from this baseline were classified as wet snow (Nagler, et al.,2016). Liquid water increases dielectric losses, reduces penetration depth, and limits volume scattering. This leads to lower backscatter, even on rough or crevassed glacier surfaces (Shi and J. Dozier 1995). Crevassed areas that show up in the wet snow class do not suggest that rough ice has been misclassified. Instead, they indicate meltwater present in the snow or firn, or along the walls of crevasses. This presence of meltwater significantly changes how radar backscattering behaves.


## Conclusions

The study shows that some of the glaciers in the third pole do not respond uniformly to climate change, and shows slightly positive mass balance for the last decades.

The focused “Kekesayi Glacier” is found to be experiencing pronounced winter warming, while summer temperatures show no significant warming trend. This seasonal asymmetry is consistent with mechanisms proposed for the Karakoram anomaly, where enhanced winter precipitation and warming contribute to sustaining glacier mass balance. The observed expansion of supraglacial lakes and moisture extent reflects evolving meltwater production and drainage dynamics, rather than a simple increase in summer melt alone.

The integration of multiple sensors (MODIS, Sentinel-1 & 2) and reanalysis products (ECMWF ERA5) can help in better understanding of evolving water balance of glaciers, and by extension, their role in regional hydrology and global climate change.

#### Future work
**Future perspectives** foresees to use newer remote sensing products such as Crystal/Sentinel 3 to measure snow depth, quantifying moisture content, differentiating debris from snow etc.

## <!--{ as="div" }--> Open Science

All datasets and platforms used in this story are freely and openly available.

| Name | Type | Agency / Provider | Description / Usage |
|---|---|---|---|
| [MODIS Land Surface Temperature (LST)](https://lpdaac.usgs.gov/products/mod11a1v061/) | Dataset | NASA / USGS | MODIS AQUA L3C daily daytime LST at 1 km resolution (2002–2018) from ESA CCI Cube. Used for analyzing seasonal and annual temperature trends over the glacier. |
| [Copernicus Sentinel-2 MSI](https://dataspace.copernicus.eu/browser/?collection=SENTINEL-2) | Dataset | ESA / Copernicus | Multispectral optical imagery at 10 m resolution for 2015, 2017, and 2020. Green and NIR bands used to calculate NDWI for supraglacial lake detection. |
| [Copernicus Sentinel-1 SAR](https://dataspace.copernicus.eu/browser/?collection=SENTINEL-1) | Dataset | ESA / Copernicus | C-band radar Ground Range Detected (GRD) data at 10 m resolution for 2015, 2017, and 2020. Used for moisture extent mapping and mass balance assessment. |
| [ECMWF ERA5 Reanalysis](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels) | Dataset | ECMWF / Copernicus | Climate reanalysis data providing temperature anomalies and precipitation context for interpreting glacier behavior. |
| [Earth System Data Lab (ESDL) — DeepESDL](https://earthsystemdatalab.net/) | Platform | Brockmann Consult / ESA | Cloud-based data cube infrastructure providing harmonized access to multiple climate data records including MODIS LST, enabling analysis of Earth system variables in a unified spatio-temporal framework. |
| [EO Dashboard](https://eodashboard.org/explore) | Platform | ESA / NASA / JAXA | Trilateral open Earth observation dashboard providing interactive access to satellite-derived datasets and stories on cryosphere, atmosphere, and land monitoring. |



#### References
- Shean, D. E., Bhushan, S., Montesano, P., Rounce, D. R., Arendt, A., & Osmanoglu, B. (2020). A systematic, regional assessment of high mountain Asia glacier mass balance. *Frontiers in Earth Science*, 7, 363.

- Salerno, F., Guyennon, N., Yang, K. et al. (2023). Local cooling and drying induced by Himalayan glaciers under global warming. *Nature Geoscience*, 16, 1120–1127. [https://doi.org/10.1038/s41561-023-01331-y](https://doi.org/10.1038/s41561-023-01331-y)

- Hugonnet, R., McNabb, R., Berthier, E. et al. (2021). Accelerated global glacier mass loss in the early twenty-first century. *Nature*, 592, 726–731. [https://doi.org/10.1038/s41586-021-03436-z](https://doi.org/10.1038/s41586-021-03436-z)

- Wangchuk, S., and Bolch, T. (2020). Mapping of glacial lakes using Sentinel-1 and Sentinel-2 data and a random forest classifier: Strengths and challenges. *Science of Remote Sensing*, 2, 100008.

- Holzer, N., Vijay, S., Yao, T., Xu, B., Buchroithner, M., and Bolch, T. (2015). Four decades of glacier variations at Muztagh Ata (eastern Pamir): a multi-sensor study including Hexagon KH-9 and Pléiades data. *The Cryosphere*, 9, 2071–2088. [https://doi.org/10.5194/tc-9-2071-2015](https://doi.org/10.5194/tc-9-2071-2015)

- Nagler, T., Rott, H., Ripper, E., Bippus, G., & Hetzenecker, M. (2016). Advancements for Snowmelt Monitoring by Means of Sentinel-1 SAR. Remote Sensing, 8(4), 348. https://doi.org/10.3390/rs8040348

- Jiancheng Shi and J. Dozier, "Inferring snow wetness using C-band data from SIR-C's polarimetric synthetic aperture radar," in IEEE Transactions on Geoscience and Remote Sensing, vol. 33, no. 4, pp. 905-914, July 1995, doi: 10.1109/36.406676 

