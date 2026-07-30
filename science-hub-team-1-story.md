---
cover-image: https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2023/10/earthcare_for_a_better_understanding_of_earth_s_radiation_balance/25154725-1-eng-GB/EarthCARE_for_a_better_understanding_of_Earth_s_radiation_balance_pillars.png
date: 2025-01-01
theme: atmosphere
tags: EarthCARE, Clouds, Atmosphere, ScienceHub
official: false

---

# Exploring our atmosphere with EarthCARE <!--{ as="img" mode="hero" src="https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2023/10/earthcare_for_a_better_understanding_of_earth_s_radiation_balance/25154725-1-eng-GB/EarthCARE_for_a_better_understanding_of_Earth_s_radiation_balance_pillars.png" }-->
### Authors: Paula Romero Jure¹ and Giacomo Roversi²³ <!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->
> ¹ University of Leeds ² Ca’ Foscari University of Venice  ³ CNR-ISAC Rome

# 
*This story is based on results from the [Science Hub Challenges in September 2025](https://sciencehub.esa.int/2025/09/29/science-hub-challenges-september-2025/) organised and hosted by ESA's ESRIN, using data from [EarthCARE satellite](https://www.esa.int/Applications/Observing_the_Earth/FutureEO/EarthCARE),  an ESA-JAXA joint mission, which was processed via the [ESA Multi-Mission Algorithm and Analysis Platform (ESA MAAP)](https://portal.maap.eo.esa.int/earthcare/), by students from the following organizations:*


##  <!--{ nav="false"}-->
<p align="center">
  <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/images.png?raw=true" alt="Ca' Foscari" height="80" style="margin: 0 15px;"/>
  <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-2/cafoscari.png?raw=true" alt="NOC" height="80" style="margin: 0 15px;"/>
  <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/logo-isac-CNR-nuovo.png?raw=true" alt="BAS" height="80" style="margin: 0 15px;"/>
</p>



## Aerosols and clouds belong together

Some clouds would not exist without aerosols, tiny particles that act as nuclei for cloud droplet formation. As air parcels rise through the troposphere, they cool, carrying water vapor that condenses around hygroscopic aerosol particles once temperatures drop enough. These particles, called Cloud Condensation Nuclei (CCN), enable liquid cloud droplets to form.

<div style="text-align: center;">
    <img src="
https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/clouds_ccns.png?raw=true " width="500"/>
    <p><b>Figure 1: CCNs </b> Schematic representation of how liquid cloud droplets form with the help of aerosol particles.</p>
</div>

Some aerosols help form ice crystals instead, acting as Ice **Nucleating Particles (INPs)**, common at higher, colder altitudes. Depending on whether droplets are liquid, ice, or both, clouds are classified as liquid, ice, or mixed-phase. Natural aerosols include sea salt, volcanic sulfates, and desert dust, while anthropogenic aerosols arise from pollution and biomass burning. 

<img src="https://upload.wikimedia.org/wikipedia/commons/3/39/Ice_Nucleation_Mechanisms.png?20141019054030" width="600" style="display:block; margin:auto;"/> <p style="text-align:center;"><b>Figure 2 </b> Various ice nucleation mechanisms in the atmosphere.
.</p>

Because aerosols influence droplet formation, they also affect cloud structure and behavior. For instance, more CCNs create numerous smaller droplets, increasing cloud reflectivity: **the Twomey effect**. By altering droplet number, phase, and thickness, aerosols modify how clouds reflect sunlight and trap heat, playing a key role in how clouds either amplify or mitigate global warming.



<img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/figure_3.jpg?raw=true" width="600" style="display:block; margin:auto;"/> <p style="text-align:center;"><b>Figure 3: Aerosols radiative effects.</b>  Aerosol particles can directly change how radiation is scattered and absorbed in the atmosphere, known as the direct effect. They can also influence cloud properties by modifying the number and size of cloud droplets or ice crystals, which in turn changes how much radiation clouds reflect. This is called the indirect aerosol effect. Source: IPCC Fourth Assessment Report 2007.</p>

<img src="https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2024/05/clouds_in_the_climate_system/26088977-1-eng-GB/Clouds_in_the_climate_system_article.png" width="600" style="display:block; margin:auto;"/> <p style="text-align:center;"><b>Figure 4: Cloud radiative effects.</b>  The amount of clouds, their height in the atmosphere and their thickness are fundamental variables that determine how they interact with the incoming and outgoing radiation.  </p>

## Challenge
We cannot continuously sample cloud droplets and aerosols directly within clouds, so researchers use several remote methods to study them. You might wonder: how did we understand clouds before satellites, and how can satellites detect such tiny particles?

Our first tool was and remains being based on developing theory. Physics helps understanding and predicting how clouds behave and interact with aerosols. Over time, scientists developed equations to describe these processes, later enhanced by computational models that simulate thousands of atmospheric equations. Though simplified, these models reveal valuable insights into cloud–aerosol interactions. To verify models, we rely on observations. In the lab, scientists study ice crystal growth or simulate clouds in controlled conditions. Aircraft equipped with specialized instruments can collect samples and measure properties in real time, but these missions are costly and limited. Satellites, on the other hand, provide continuous, global coverage that complements models, lab work, and field campaigns. Together, these tools offer a more complete picture of this complex system, helping us improve weather and climate predictions in a warming world.

## Objective

The objective of this study is to explore whether and how aerosols influence cloud characteristics: specifically the distribution of liquid water and ice content, at various altitudes using EarthCare’s vertical profiling capabilities. To this end, **EarthCare**,  a mission realised through a joint venture between the [European Space Agency (ESA)](esa.int) and the [Japan Aerospace Exploration Agency (JAXA)](https://global.jaxa.jp/), was used to identifying patterns in cloud-aerosol interactions across different regions and conditions (e.g. land vs. ocean, tropical vs. polar environments), and determining whether increased CCN or INP concentrations correlate with observable changes in cloud composition.


<div style="text-align: center;"> <img src="https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2024/01/earthcare_over_desert_dust/25391626-1-eng-GB/EarthCARE_over_desert_dust_pillars.png" width="800"/> <p><b>Figure 5.</b> EarthCare Satellite (source: ESA).</p> </div>

#### Why EarthCare? 

EarthCARE is a first-of-its-kind mission that offers an opportunity to understand the complexity of cloud changes using a single satellite. What makes EarthCARE special is its four instruments working together to study clouds, aerosols, and radiation in detail.


* **ATLID (Atmospheric Lidar)** uses laser pulses to detect aerosols and thin cloud layers by measuring how light scatters back from particles, providing high-resolution profiles that improve on previous lidar missions like CALIPSO.
* **CPR (Cloud Profiling Radar)** can "see" across the clouds with radar signals to measure their vertical structure and water content, adding the capability to capture cloud motion and the fall speed of precipitation. This improves the previous mission called CloudSat.
* **MSI (Multi-Spectral Imager)** delivers multi-wavelength images in 7 different bands that reveal cloud structure and aerosol distribution over large areas, complementing with higher spatial resolution. The product resolution of MODIS is 250m/500/1km, while the MSI is 500m.
 [MODIS](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/modis/) with higher spatial resolution. The product resolution of MODIS is 250m/500/1km, while the MSI is 500m. 
* **BBR (Broadband Radiometer)** measures solar and thermal radiation reflected and emitted by Earth, enabling direct estimates of top-of-atmosphere radiative effects and energy balance.


<div style="text-align: center;"> <img src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/team1-earthcare-sensors-image.png?raw=true" width="800"/> <p><b>Figure 6.</b> EarthCare Satellite (source: ESA).</p> </div>



## Use cases
In the latest ESA challenge workshop, we set out to explore the clouds and aerosols at three different locations with quite special characteristics. Just near the Equator lies a very characteristic and dynamic region called the Inter-Tropical Convergence Zone (ITCZ) that stretches across the globe, a narrow belt in the troposphere characterized by persistent clouds with high and icy tops. The formation of the ITCZ is driven by the warm and moist air that is heated-up by the sun, and then ascends and cools forming clouds. Two of the areas we chose to study are within the ITCZ, one in the West Pacific Ocean and the other one in the East Pacific Ocean. The third  region is in Antarctica,in  the Southern Ocean. Here the conditions are quite different and clouds are lower, but because of the low temperature, these are mostly made of supercooled liquid water, and sometimes ice.

<div style="text-align: center;">
    <img src="
https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/Globe1_pacific.png?raw=true  " width="500"/>
    <p><b>Figure 7: Locations to study. </b> The three locations of our study for the ESA challenge.</p>
</div>

##  <!--{ nav="false"}-->## use cases <!--{ as="eox-map" mode="tour" }-->
### <!--{ layers='[{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"cloudless-2024;:;EPSG:3857","title":"EOxCloudless 2024"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2024_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ EOxCloudless 2024: <a xmlns:dct=\"http://purl.org/dc/terms/\" href=\"https://s2maps.eu\" target=\"_blank\" property=\"dct:title\">Sentinel-2 cloudless - s2maps.eu</a> by <a xmlns:cc=\"http://creativecommons.org/ns#\" href=\"https://eox.at\" target=\"_blank\" property=\"cc:attributionName\" rel=\"cc:attributionURL\">EOX IT Services GmbH</a> (Contains modified Copernicus Sentinel data 2024) }"},"preload":null},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null},{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"WebGLTile","source":{"type":"GeoTIFF","normalize":false,"interpolate":false,"sources":[{"url":"https://workspace-ui-public.dashboards-operations.aws.hub.eox.at/api/public/share/public-708aab981-1a/earthCARE_Team1SienceHub25/ECA_MSI_1B_20250616.tif"}]},"properties":{"id":"earthCARE_MSI;:;2025-06-16T00:00:00Z;:;0","title":"earthCARE_MSI_20250616"},"style":{"color":["case",[">",["band",1],0],["interpolate",["linear"],["band",1],8,[0,0,0,1],265,[255,255,255,1]],[0,0,0,0]]}},{"type":"Vector","source":{"type":"Vector","url":"https://workspace-ui-public.dashboards-operations.aws.hub.eox.at/api/public/share/public-708aab981-1a/earthCARE_Team1SienceHub25/ECA_EXAD_AC__TC__2B_20250616T202420Z_20250616T233239Z_05973E.geojson","format":{"type":"GeoJSON","dataProjection":"EPSG:4326"}},"properties":{"id":"EarthCARE_orbit_track;:;2025-06-16T00:00:00Z;:;0","title":"EarthCARE_orbit_track_20250616","layerDatetime":{"controlValues":["2025-06-16T00:00:00.000Z","2025-06-21T00:00:00.000Z","2025-06-28T00:00:00.000Z"],"currentStep":"2025-06-16T00:00:00.000Z","slider":true,"navigation":true,"play":false,"displayFormat":"DD.MM.YYYY HH:mm","animateOnClickInterval":false},"color":"#009E73","timeControlValues":[{"itemId":"2025-06-16T00:00:00Z","date":"2025-06-16T00:00:00.000Z"},{"itemId":"2025-06-21T00:00:00Z","date":"2025-06-21T00:00:00.000Z"},{"itemId":"2025-06-28T00:00:00Z","date":"2025-06-28T00:00:00.000Z"}],"timeControlProperty":"TIME","layerControlExpand":true,"layerControlToolsExpand":true},"style":{"stroke-color":"#ff0000","stroke-width":10},"interactions":[]}]},{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857","attributions":"{ Overlay: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors, Made with Natural Earth, Rendering &copy; <a href=\"https://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]}]' zoom="6.9" center=[-98.54392824360147,10.5] projection="" animationOptions={duration:500}}-->
#### EarthCARE acquisitions: 3 dates and locations
The **red line** marks the **satellite's ground track for that orbit**, for each date and use case selected for this study.

The **grayscale image underneath shows EarthCARE's MSI visible channel (0.67 µm)** Level-1B acquisition (from June 16, 2025), displaying top-of-atmosphere reflectance. Brighter areas indicate higher reflectance, typically corresponding to thick clouds or bright surfaces, while darker areas represent ocean or cloud-free regions. 




### <!--{ layers='[{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"cloudless-2024;:;EPSG:3857","title":"EOxCloudless 2024"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2024_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ EOxCloudless 2024: <a xmlns:dct=\"http://purl.org/dc/terms/\" href=\"https://s2maps.eu\" target=\"_blank\" property=\"dct:title\">Sentinel-2 cloudless - s2maps.eu</a> by <a xmlns:cc=\"http://creativecommons.org/ns#\" href=\"https://eox.at\" target=\"_blank\" property=\"cc:attributionName\" rel=\"cc:attributionURL\">EOX IT Services GmbH</a> (Contains modified Copernicus Sentinel data 2024) }"},"preload":null},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null},{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Vector","source":{"type":"Vector","url":"https://workspace-ui-public.dashboards-operations.aws.hub.eox.at/api/public/share/public-708aab981-1a/earthCARE_Team1SienceHub25/ECA_EXAD_AC__TC__2B_20250616T202420Z_20250616T233239Z_05973E.geojson","format":{"type":"GeoJSON","dataProjection":"EPSG:4326"}},"properties":{"id":"EarthCARE_orbit_track;:;2025-06-16T00:00:00Z;:;0","title":"EarthCARE_orbit_track_20250616"},"style":{"stroke-color":"#ff0000","stroke-width":10}}]},{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857","attributions":"{ Overlay: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors, Made with Natural Earth, Rendering &copy; <a href=\"https://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]}]' zoom="4.501631437033822" center=[-70.9112386063985,0.006852185440251901] projection="" animationOptions={duration:500}}-->
#### Eastern Pacific
In this region, being far from major population centers, we expect fewer aerosol sources. In terms of the climatology, this region is characterized by large-scale subsidence, where air is drier than in the west, as the sea temperature is colder than in the West in normal conditions. Figure explains the regional differences in the climate pattern in the Pacific due to the characteristic Walker circulation.

<div style="text-align: center;">
    <img src="https://catalog.maap.eo.esa.int/data/earthcare-pdgs-01/EarthCARE/AC__TC__2B/AD/2025/06/28/ECA_EXAD_AC__TC__2B_20250628T152631Z_20250628T174754Z_06157A/public/ECA_EXAD_AC__TC__2B_20250628T152631Z_20250628T174754Z_06157A.BID_0.jpeg" width="500"/>
    <p><b>Figure 10</b>: Synergetic Target Classification profile from EarthCARE for 28-06-2025.</p>
</div>







### <!--{ layers='[{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"cloudless-2024;:;EPSG:3857","title":"EOxCloudless 2024"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2024_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ EOxCloudless 2024: <a xmlns:dct=\"http://purl.org/dc/terms/\" href=\"https://s2maps.eu\" target=\"_blank\" property=\"dct:title\">Sentinel-2 cloudless - s2maps.eu</a> by <a xmlns:cc=\"http://creativecommons.org/ns#\" href=\"https://eox.at\" target=\"_blank\" property=\"cc:attributionName\" rel=\"cc:attributionURL\">EOX IT Services GmbH</a> (Contains modified Copernicus Sentinel data 2024) }"},"preload":null},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null},{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Vector","source":{"type":"Vector","url":"https://workspace-ui-public.dashboards-operations.aws.hub.eox.at/api/public/share/public-708aab981-1a/earthCARE_Team1SienceHub25/ECA_EXAD_AC__TC__2B_20250621T010314Z_20250621T035704Z_06038G.geojson","format":{"type":"GeoJSON","dataProjection":"EPSG:4326"}},"properties":{"id":"EarthCARE_orbit_track;:;2025-06-21T00:00:00Z;:;0","title":"EarthCARE_orbit_track_20250621"},"style":{"stroke-color":"#ff0000","stroke-width":10}}]},{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857","attributions":"{ Overlay: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors, Made with Natural Earth, Rendering &copy; <a href=\"https://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]}]' zoom="2.9856040433774247" center=[124.71035954823785,-69.30818362670098] projection="" animationOptions={duration:500}}-->
#### Southern Ocean
Aerosols might potentially be carried from far away, and influence cloud formation here. We mostly expect sea salt aerosols, but there could also be stratospheric aerosols, especially from volcanic eruptions. The atmospheric dynamics are quite particular in this region. Supercooled liquid clouds and ice clouds form at much lower altitudes compared to what happens in latitudes closer to the Equator, given the low temperature of the atmosphere.

<div style="text-align: center;">
    <img src="
https://catalog.maap.eo.esa.int/data/earthcare-pdgs-01/EarthCARE/AC__TC__2B/AD/2025/06/21/ECA_EXAD_AC__TC__2B_20250621T010314Z_20250621T035704Z_06038G/public/ECA_EXAD_AC__TC__2B_20250621T010314Z_20250621T035704Z_06038G.BID_0.jpeg" width="500"/>
    <p><b>Figure 9</b>: Synergetic Target Classification profile from EarthCARE for 21-06-2025.</p>
</div>




### <!--{ layers='[{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"cloudless-2024;:;EPSG:3857","title":"EOxCloudless 2024"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2024_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ EOxCloudless 2024: <a xmlns:dct=\"http://purl.org/dc/terms/\" href=\"https://s2maps.eu\" target=\"_blank\" property=\"dct:title\">Sentinel-2 cloudless - s2maps.eu</a> by <a xmlns:cc=\"http://creativecommons.org/ns#\" href=\"https://eox.at\" target=\"_blank\" property=\"cc:attributionName\" rel=\"cc:attributionURL\">EOX IT Services GmbH</a> (Contains modified Copernicus Sentinel data 2024) }"},"preload":null},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null},{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857","attributions":"{ OSM: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors and <a href=\"https://maps.eox.at/#data\" target=\"_blank\">others</a>, Rendering &copy; <a href=\"http://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Vector","source":{"type":"Vector","url":"https://workspace-ui-public.dashboards-operations.aws.hub.eox.at/api/public/share/public-708aab981-1a/earthCARE_Team1SienceHub25/ECA_EXAD_AC__TC__2B_20250628T152631Z_20250628T174754Z_06157A.geojson","format":{"type":"GeoJSON","dataProjection":"EPSG:4326"}},"properties":{"id":"EarthCARE_orbit_track;:;2025-06-28T00:00:00Z;:;0","title":"EarthCARE_orbit_track_20250628"},"style":{"stroke-color":"#ff0000","stroke-width":10}}]},{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"https://{a-e}.s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857","attributions":"{ Overlay: Data &copy; <a href=\"http://www.openstreetmap.org/copyright\" target=\"_blank\">OpenStreetMap</a> contributors, Made with Natural Earth, Rendering &copy; <a href=\"https://eox.at\" target=\"_blank\">EOX</a> }"},"preload":null}]}]' zoom="4.558748207255449" center=[135.04552392610523,-0.008759548153335572] projection="" animationOptions={duration:500}}-->
#### West Pacific (ITCZ)
The western ITCZ is very interesting because of the potential sources of aerosols that we could find in the area. First, we have the characteristic strong updrafts (air moving upwards) of the ITCZ, but here the storms can be exceptionally strong and stir the ocean, lifting sea salt aerosols into the atmosphere. These are natural aerosols (non-anthropogenic). However, nearby regions such as Southeast Asia and China may contribute with anthropogenic aerosols derived from human activities, like pollution or industrial activity, or with aerosols that come from biomass burn.


<div style="text-align: center;">
    <img src="https://catalog.maap.eo.esa.int/data/earthcare-pdgs-01/EarthCARE/AC__TC__2B/AD/2025/06/16/ECA_EXAD_AC__TC__2B_20250616T202420Z_20250616T233239Z_05973E/public/ECA_EXAD_AC__TC__2B_20250616T202420Z_20250616T233239Z_05973E.BID_0.jpeg" width="500"/>
    <p><b>Figure 8</b>: Synergetic Target Classification profile from EarthCARE for 16-06-2025.</p>
</div>

This profile combines ATLID and CPR data to classify the atmosphere from surface to 20 km. In this study, this classification product (AC__TC__2B Synergetic Target Classification profile from EarthCARE) was one of the datasets used to interpret which cloud regimes (liquid, ice, or mixed-phase) drove the observed aerosol–cloud relationships.</p>

 
 
 

##
Comparing these three very interesting regions with quite distinctive characteristics could give us a hint on whether the aerosols are influencing changes in the clouds.
<div style="text-align: center;">
    <img src="
https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/Screenshot%20from%202025-11-06%2012-12-20.png?raw=true" width="500"/>
    <p><b>Figure 11:  The Walker circulation. </b> Normal Pacific conditions (Walker circulation) feature warm western waters with rising air and convection, and cool eastern waters with sinking air, producing east-to-west trade winds. Credit: [David Babb @ Penn State is licensed under CC-BY-NC-4.0](https://www.e-education.psu.edu/meteo3/node/2273).</p>
</div>





## Data and Methods
We used data derived from two instruments out of the four on-board EarthCARE, which can provide a vertical profiling of the atmosphere:
- **Cloud Profiling Radar (CPR)**: 94 GHz nadir-viewing radar with ~750m horizontal resolution and 500m vertical resolution, providing cloud structure and water content.
- **Atmospheric Lidar (ATLID)**: 354.8 nm nadir-viewing lidar with <30m horizontal resolution. The vertical resolution is 103m (below 20.2km altitude) and 500 m (above 20.2km altitude), detecting aerosols and thin clouds.

#### Dataset
The analysis used three primary EarthCARE data products:
- **CPR_CLD_2A**: Cloud variables including Liquid Water Path (LWP) and Ice Water Path (IWP), plus land/ocean flags
- **ATL_ALD_2A**: Aerosol Optical Thickness (AOT) at 355nm from lidar measurements
- **AC_TC_2A**: Synergistic radar-lidar target classification distinguishing cloud types and aerosol layers

Data coverage: The analysis was conducted using approximately 600-700 scenes from June-July and September 2025, limited by early mission data availability. The code was run using the [ESA Multi-Mission Algorithm and Analysis Platform (ESA MAAP)](https://portal.maap.eo.esa.int/earthcare/).

#### Methodology workflow

The analysis followed a systematic processing pipeline:
* **1- Extract** the available data: This step involved selecting the scenes of interest from the EarthCARE dataset. At the time of conducting the analysis, between 600 and 700 scenes were available for the target regions.
* **2- Resample** data at 1-second temporal resolution: Since the radar and lidar often record data at intervals shorter than one second, we standardised the temporal resolution by averaging all values within each 1‑second window.
* **3- Merge** datasets: We combine variables from multiple instruments together. We merge the Aerosol Optical Thickness (from Lidar), the Liquid Water Path and Ice Water Path (from radar) and the Target classification (from both radar and lidar) at 1-second temporal resolution.
* **4- Resample** to 1-minute temporal resolution: For simplicity, the merged dataset was further averaged into 1‑minute intervals, applying a mean across each variable within each minute.
* **5- Select** months with **complete** data available: The analysis focused on June, July, and September 2025, as these were the months for which full datasets of the three variables were available.
* **5- Normalize**  variables: Prior to model training, each variable was normalised using a min–max scaling approach x' = x -xminxmax-xmin , where x is a variable value, xmin is the minimum value observed for that variable within the selected data and xmax is the maximum value.
* **6 - Clustering** approach: A K‑means clustering algorithm was applied with the aim of grouping the data and, from there, explore relationships between variables. As this is an unsupervised method, the number of clusters must be specified in advance. We used the elbow method to determine the optimal number of clusters, which was found to be five (see Figure 9).

Finally, the synergetic product provided insights on the types of clouds or aerosols that are grouped on each cluster.


<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/elbow_graph.jpg?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Pacific region clusters"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 12: Data points indicating their assigned clusters</b>  The resulting clustering, expressed by different colours, is shown for the West Pacific (upper row) and the East Pacific (bottom row). 
    </p>
</div>



**Limitations**: Not all EarthCARE data products are yet available, and merging different instruments (particularly MSI with CPR and ATLID) remains challenging in early mission phases. Also, this is only an exploratory analysis, in which we explore possible broad relations between variables. 

## Results
Although this was only an exploratory analysis, several interesting insights emerge. The following figures show the data points from each product in each study region, resampled to 1‑minute resolution. Each figure therefore represents the output after applying the processing pipeline up to <b>Step 5</b>. Each axis corresponds to one of the variables used in the study. The resulting clusters are shown as different colours, where each colour represents the assigned cluster for a given data point, and the red crosses indicate the cluster centroids.

<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/results1_team1.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Pacific region clusters"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 13: Data points indicating their assigned clusters</b>  The resulting clustering, expressed by different colours, is shown for the West Pacific (upper row) and the East Pacific (bottom row). 
    </p>
</div>

Looking more closely at the ice water path (IWP) versus aerosol optical thickness (AOT) panels (Fig. 13 a and d), many points fall either along the line where <b>IWP = 0</b> or where <b>AOT = 0</b>. This behaviour is expected: aerosols are measured by the lidar, and thick ice‑topped clouds (high IWP) strongly attenuate the lidar signal, preventing aerosol retrievals. However, it is notable that some points show non‑zero values for both variables. This suggests that there may be conditions under which both aerosol and ice‑cloud properties can be detected simultaneously, which warrants further investigation.

Focusing on the first panel for the West Pacific (Fig. 13a), there are data points in the region where <b>IWP > 0.2 kg m⁻³</b>, which is considered indicative of thick ice clouds, and <b>AOT > 0</b>. The majority of these points are classified as cluster 3 (green dots), with a smaller number belonging to cluster 4 (orange dots).

In the East Pacific (Fig.10d), the distribution of the data points is broadly similar to the West Pacific (Fig. 13a). Curiously, the clusters are inverted: cluster 4 (orange dots) are the points with high IWP values and cluster 3 (green dots) represent points with high AOT values. A few values classified as cluster 1 (blue dots) , with noticeable values of <b>IWP >0</b> and <b>AOT>0</b> emerge in the East Pacific. In the West, this cluster is not so significant. 

Examining Fig. 13b, which shows <b>LWP versus AOT</b> for the West Pacific, we observe that most data points in cluster 3 (green dots) exhibit lower LWP values compared to their IWP values. By contrast, in cluster 4 (orange dots), LWP is higher than IWP for the same AOT values.

Looking next at the <b>LWP versus IWP</b> plot (Fig. 13c), we confirm that cluster 3 data points (green dots) mainly represent thick ice clouds, while cluster 4 points (orange dots) are predominantly composed of liquid water. Another notable group is cluster 2, shown as light‑blue points, which displays mixed characteristics: several points have significant values of both LWP and IWP, potentially representing mixed‑phase clouds. The relationship with AOT is much stronger for the liquid phase (Fig. 10b) than for the ice phase (Fig. 13a), although a few light‑blue outliers exhibit <b>IWP > 0.2 kg m⁻³</b> together with <b>AOT > 0</b>.

In the East Pacific, we observe a broadly similar distribution of data points to that of the West Pacific. However, there are many more points and clusters for which LWP values (Fig. 13e) are higher than those seen in the West Pacific. This difference may partly arise from measurement artefacts. In the West Pacific, high clouds tend to have higher and colder tops and to be more spatially extensive than in the East Pacific. As a result, lidar attenuation can occur over much larger vertical and horizontal scales. Consequently, even if aerosol burdens are actually higher in the West Pacific, these cloud‑regime differences must be taken into account.

Overall, the East Pacific shows a larger occurrence of liquid‑phase clouds (Fig. 13e) than the West Pacific, for which clearer relationships with aerosols are observed, as these clouds are generally located at lower altitudes. Because cloud properties and phases are derived primarily from radar observations, stronger confidence can be placed in these conclusions. Moreover, Fig. 10f suggests a higher occurrence of mixed‑phase clouds in the East Pacific, which may be more likely to interact with aerosols.

The data points for the Southern Ocean region are shown in  <b>Figure 14</b>, where a much more pristine environment is evident. The majority of data points correspond to ice clouds: in the third panel, all points show LWP = 0, except for a single outlier. No clear relationship between IWP and AOT is evident in the first panel, again with only one outlier that would require further investigation. This is likely due to strong lidar attenuation by ice clouds, an effect that is even more pronounced than in the tropics. As shown here, Southern Ocean clouds are predominantly ice‑phase, with very limited liquid or mixed‑phase occurrence.


<div style="display: flex; flex-direction: column; align-items: center; margin: 40px 0;">
    <img 
        src="https://github.com/eurodatacube/eodash-assets/blob/main/stories/ScienceHub-Challenge-September-2025/Team-1/results3_team1.png?raw=true" 
        style="max-width: 100%; width: 800px; height: auto;"
        alt="Spatial cluster distribution"
    />
    <p style="text-align: center; font-size: 1.2em; margin-top: 10px;">
        <b>Figure 14: Clustering results in Antartica. </b> Compared to the results in the Tropical Pacific, we didn't find many aerosol-clouds relations due to the lidar attenuation in ice clouds.
    </p>
</div>


## Conclusions

This study demonstrates the capability of EarthCARE's integrated sensor suite to reveal relationships between aerosol properties and cloud microphysics across different climate regions. From this exploratory analysis, several insights emerge regarding the connections between aerosols and cloud properties, as observed by EarthCARE.

First, aerosol–cloud relationships are strongly modulated by cloud phase and vertical structure. In all regions analysed, the most clear relationships between aerosol optical thickness (AOT) and cloud properties are primarily observed for liquid clouds, and some for and mixed‑phase clouds. Such relationships are much weaker for ice‑dominated clouds. Although this could be a physical signal, it mostly reflects observational constraints: ice clouds strongly attenuate the lidar signal, limiting aerosol detectability beneath or within these clouds. This happens for both thick clouds with ice-made tops in the tropics, but also for some thinner clouds made of ice in the Southern Ocean. 

Understanding of regional cloud regimes play a critical role in the interpretation of the observed aerosol–cloud connections. This is particularly relevant across the ITCZ, where regimes can be quite different. 
In spite of the natural observational constraints, the clustering analysis reveals promising information regarding cloud-aerosol interactions. The identified clusters consistently distinguish between ice‑dominated, liquid‑dominated, and mixed‑phase cloud populations, each exhibiting different sensitivities to aerosol presence. This demonstrates the value of combining radar‑derived cloud properties with lidar‑based aerosol retrievals.

Further analysis should include the synergetic product, which would aid with the understanding of not only the cloud regimes but also the type of aerosol. By relating the clusters obtained to the different species of aerosols obtained, we can get better insights on the aerosol distributions on each region and the interactions with clouds. 
 


## <!--{ as="div" }--> Open Science

| **Name**                                                                                                                                       | **Type**            | **Agency / Provider**                     | **Description / Usage**                                                                                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **[EarthCARE Mission](https://www.esa.int/Applications/Observing_the_Earth/FutureEO/EarthCARE)**                                        | Mission/Platform             | ESA/JAXA               | Earth Cloud, Aerosol and Radiation Explorer satellite providing integrated observations from Cloud Profiling Radar, Atmospheric Lidar, Multi-Spectral Imager, and Broad Band Radiometer.                            |
| **[CPR_CLD_2A Product](https://www.eoportal.org/satellite-missions/earthcare#sensor-complement)**                                                                                       | Dataset | ESA/JAXA                        | Cloud Profiling Radar Level 2A product providing cloud variables, Liquid Water Path (LWP), Ice Water Path (IWP), and land/ocean flags.                                     |
| **[ATL_ALD_2A Product](https://amt.copernicus.org/preprints/amt-2023-252/)**                                          | Dataset     | ESA/JAXA               | Atmospheric Lidar Level 2A product providing Aerosol Optical Thickness (AOT) at 355nm and aerosol layer properties.                                                     |
| **[AC_TC_2A Product](https://www.eoportal.org/satellite-missions/earthcare#sensor-complement)**                          | Dataset | ESA/JAXA | Synergistic radar-lidar target classification product distinguishing cloud types and aerosol layers.                                               |
| **[ESA MAAP – ESA Multi-Mission Algorithm and Analysis Platform](https://portal.maap.eo.esa.int/earthcare/)**                          | Platform | ESA | Cloud-based platform for processing and analyzing Earth observation data, used for EarthCARE data processing and clustering analysis.                                               |
#### Notebook
Access the notebook to reproduce the study workflow.
<iframe width="100%" height="600" src="https://esa-eodashboards.github.io/eodashboard-notebooks/notebooks/openchallangenotebook-earthcare-cloud-aerosols-int/" frameborder="0"></iframe>




#### References
- Finney, D. L., et al. (2025). *Microphysical fingerprints in anvil cloud albedo*. Journal of the Atmospheric Sciences. https://egusphere.copernicus.org/preprints/2025/egusphere-2025-1227/

- Lorian, A., et al. (2023). *Aerosol effects on deep convection: A review*. Atmospheric Research. https://doi.org/10.1016/j.atmosres.2023.xxxxx
  <!-- Verify DOI: the ACP DOI in the original citation belongs to a different paper -->

- Grabowski, W. W., & Morrison, H. (2016). *Untangling microphysical impacts on deep convection applying a novel modeling methodology*. Journal of the Atmospheric Sciences, 73(6), 2503–2524. https://doi.org/10.1175/JAS-D-14-0307.1

- Heikenfeld, M., et al. (2019). *Aerosol effects on deep convection: The propagation of aerosol perturbations through convective cloud microphysics*. Atmospheric Chemistry and Physics, 19(4), 2601–2627. https://doi.org/10.5194/acp-19-2601-2019

- Igel, A. L., & van den Heever, S. C. (2021). *The relative influence of environmental characteristics on tropical deep convective morphology as observed by CloudSat*. Journal of Geophysical Research: Atmospheres, 126(6). https://doi.org/10.1029/2020JD033811

- [Mi, Jiaqin & Yang, Yuanjian & Zhou, Shuxue & Ma, Xiaoyan & Wei, Siying. (2024). Exploring impacts of aerosol on convective clouds using satellite remote sensing and machine learning. Journal of Applied Remote Sensing. 18. 10.1117/1.JRS.18.012007.](https://www.researchgate.net/publication/377380698_Exploring_impacts_of_aerosol_on_convective_clouds_using_satellite_remote_sensing_and_machine_learning)

- [AMT - Cloud top heights and aerosol layer properties from EarthCARE lidar observations](https://amt.copernicus.org/preprints/amt-2023-252/)

- [GMD - Estimation of aerosol and cloud radiative heating rate in the tropical stratosphere using a radiative kernel method](https://gmd.copernicus.org/)

- [Wildfires in Southeast Asia pollute the atmosphere in the northern South China Sea](https://www.sciencedirect.com/)

- [Copernicus - Wildfires 2025 review: ASEAN reduces emissions, but haze persists](https://atmosphere.copernicus.eu/)

####  Contributors
Filippo Calì Quaglia (Ca' Foscari University, Venice)


