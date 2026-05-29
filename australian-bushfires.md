---
cover-image: https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/8-wildfires.jpg
date: 2025-01-01
theme: atmosphere
tags: wildfires,forests,no2,co2
official: true
collections: N1_CO, N1_NO2, N1_SO2
---

#  Australian bushfires in 2019-2020 emitted 700 million metric tons of CO2 into the atmosphere <!--{ as="img" mode="hero" src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/8-wildfires.jpg" }-->
### How Air Pollution affects Climate Change <!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->

## <!--{ nav="false" }-->
<div align="center">

*This trilateral story, produced in collaboration by the [European Space Agency (ESA)](https://www.esa.int), the [National Aeronautics and Space Administration (NASA)](https://www.nasa.gov/), and the [Japan Aerospace Exploration Agency (JAXA)](https://global.jaxa.jp/), is part of the joint narratives featured on [EO Dashboard](https://eodashboard.org/), showcasing the power of open Earth observation data.*

</div>


  ## <!--{ nav="false" }-->
<p align="center">
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/refs/heads/main/logos/esa.jpg" alt="ESA" height="80" style="margin: 0 15px;"/>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/refs/heads/main/logos/nasa.jpeg" alt="NASA" height="80" style="margin: 0 15px;"/>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash-assets/refs/heads/main/logos/jaxa.jpeg" alt="JAXA" height="80" style="margin: 0 15px;"/>
</p>

## Air Pollution and Climate Change

Australia’s bushfires in the 2019-2020 season emitted about 700 million tonnes of carbon dioxide into the atmosphere. Using satellite data, a new study published in Nature proves how satellite measurements can illuminate the complicated ways in which Earth is responding to climate change in an era of worsening wildfires.

Australia is no stranger to bushfires, however, the 2019-2020 season proved to be unprecedented. As of March 2020, the fires burned an estimated 18.6 million hectares (or 186 000 sq km) destroying over 5000 buildings and killing over 400 people. It was estimated that more than a billion animals perished from the bushfires, with several endangered species facing the risk of total extinction.

Based on a new [paper](https://www.nature.com/articles/s41586-021-03712-y), published in _Nature_, the extreme bushfires across southeast Australia released about 700 million tonnes of carbon dioxide into the air – more than double the emissions provided by fire emission inventory datasets.

In southeast Australia, the fires were both intense and extensive. As much as 74 000 sq km of mostly eucalyptus forest, roughly 2.5 times the area of Belgium, was affected. Previous estimates from global inventory datasets of wildfire emissions based on satellite fire data and modelled quantities of standing biomass suggested that the fires released on average 275 million tonnes of carbon dioxide between November 2019 and January 2020.

However, the new analysis indicates that this figure was a gross underestimate. Using measurements from the Tropomi instrument on board the Copernicus Sentinel-5P satellite more accurate estimates of the emissions were obtained.

<center>
<figure>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/Carbon_monoxide_from_fires_in_Australia_article.jpg" >
  <figcaption>This image uses information from the Copernicus Sentinel-5P mission and shows the average carbon monoxide concentrations from 1 November 2019 to 31 January 2020. Carbon monoxide is commonly associated with traffic, but the concentrations here are due to the bushfires. Naturally, once in the air, it can cause problems for humans by reducing the amount of oxygen that can be transported in the bloodstream. Copyright: contains modified Copernicus Sentinel data (2019-20), processed by ESA.</figcaption>
</figure>


## Copernicus Sentinel-5p TROPOMI
 
While Tropomi doesn’t directly measure carbon dioxide, the instrument takes daily snapshots of carbon monoxide levels in the atmospheric column beneath it. These data have been used to calculate a detailed estimate of the carbon monoxide emissions from the bushfires, which were then used as a proxy for calculating carbon dioxide emissions.

The conclusion is that the bushfires released about 700 million tonnes in just three months. This is twice the amount of carbon dioxide that had previously been suggested by fire inventory estimates and surpasses Australia’s normal annual bushfire and fossil fuel emissions by 80%.

<center>
<figure>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/Monitoring_air_quality_pillars.jpg" >
  <figcaption>Sentinel-5 Precursor is the first Copernicus mission dedicated to monitoring our atmosphere. This satellite carries the state-of-the-art Tropomi instrument to map a multitude of trace gases such as nitrogen dioxide, ozone, formaldehyde, methane, carbon monoxide and aerosols – all of which affect the air we breathe and our climate. Source: esa.int.</figcaption>
</figure>

## Explore Datasets

This **EO Dashboard** provides access to interactive maps of Carbon Monoxide, Nitrogen Dioxide, and Sulfur Dioxide from TROPOMI. Access these datasets by clicking on the [Dashboard](https://eodashboard.org/explore) button at the top of the page or directly from the links below:

- [TROPOMI CO](https://eodashboard.org/explore?indicator=N1_CO)
- [TROPOMI NO2](https://eodashboard.org/explore?indicator=N1_NO2)  
- [TROPOMI SO2](https://eodashboard.org/explore?indicator=N1_SO2)

The compare feature in the dashboard allows looking at the levels of CO on two different dates or compare two variables on similar dates.


## Map Tour Example <!--{ as="eox-map" mode="tour" }-->
### <!--{ layers='[{"type":"Tile","properties":{"id":"Terrain light"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpg"]}},{"type":"Tile","properties":{"id":"CO_3_daily-2019-11-03T00:00:00Z"},"source":{"type":"TileWMS","urls":["https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54"],"params":{"layers":"AWS_VIS_CO_3DAILY_DATA","styles":"","format":"image/png","time":"2019-11-03T00:00:00Z"}}},{"type":"Tile","properties":{"id":"Overlay labels"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.jpg"]}}]' zoom="4.391928094887362" center=[128.1361269438078,-31.53688018319827] animationOptions={duration:500}}-->
#### 03 November 2019 
Copernicus Sentinel-5P TROPOMI observations of Carbon Monoxide over Australia. 
The beginning of the bushfires in Eastern Australia is visible.
	
### <!--{ layers='[{"type":"Tile","properties":{"id":"Terrain light"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpg"]}},{"type":"Tile","properties":{"id":"CO_3_daily-2019-11-05T00:00:00Z"},"source":{"type":"TileWMS","urls":["https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54"],"params":{"layers":"AWS_VIS_CO_3DAILY_DATA","styles":"","format":"image/png","time":"2019-11-05T00:00:00Z"}}},{"type":"Tile","properties":{"id":"Overlay labels"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.jpg"]}}]' zoom="4.391928094887362" center=[128.1361269438078,-31.53688018319827] animationOptions={duration:500}}-->
#### 05 November 2019
This image taken just 2 days after shows the rapid extent of the fires
### <!--{ layers='[{"type":"Tile","properties":{"id":"Terrain light"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpg"]}},{"type":"Tile","properties":{"id":"CO_3_daily-2019-11-06T00:00:00Z"},"source":{"type":"TileWMS","urls":["https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54"],"params":{"layers":"AWS_VIS_CO_3DAILY_DATA","styles":"","format":"image/png","time":"2019-11-06T00:00:00Z"}}},{"type":"Tile","properties":{"id":"Overlay labels"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.jpg"]}}]' zoom="4.391928094887362" center=[128.1361269438078,-31.53688018319827] animationOptions={duration:500}}-->
#### 06 November 2019
	
Scroll to visualise further dates and see the evolution of the emissions
	
### <!--{ layers='[{"type":"Tile","properties":{"id":"Terrain light"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpg"]}},{"type":"Tile","properties":{"id":"CO_3_daily-2019-11-07T00:00:00Z"},"source":{"type":"TileWMS","urls":["https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54"],"params":{"layers":"AWS_VIS_CO_3DAILY_DATA","styles":"","format":"image/png","time":"2019-11-07T00:00:00Z"}}},{"type":"Tile","properties":{"id":"Overlay labels"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.jpg"]}}]' zoom="4.391928094887362" center=[128.1361269438078,-31.53688018319827] animationOptions={duration:500}}-->
#### 07 November 2019
### <!--{ layers='[{"type":"Tile","properties":{"id":"Terrain light"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpg"]}},{"type":"Tile","properties":{"id":"CO_3_daily-2019-11-08T00:00:00Z"},"source":{"type":"TileWMS","urls":["https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54"],"params":{"layers":"AWS_VIS_CO_3DAILY_DATA","styles":"","format":"image/png","time":"2019-11-08T00:00:00Z"}}},{"type":"Tile","properties":{"id":"Overlay labels"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.jpg"]}}]' zoom="4.391928094887362" center=[128.1361269438078,-31.53688018319827] animationOptions={duration:500}}-->
#### 08 November 2019

### <!--{ layers='[{"type":"Tile","properties":{"id":"Terrain light"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpg"]}},{"type":"Tile","properties":{"id":"CO_3_daily-2019-11-09T00:00:00Z"},"source":{"type":"TileWMS","urls":["https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54"],"params":{"layers":"AWS_VIS_CO_3DAILY_DATA","styles":"","format":"image/png","time":"2019-11-09T00:00:00Z"}}},{"type":"Tile","properties":{"id":"Overlay labels"},"source":{"type":"XYZ","urls":["//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.jpg"]}}]' zoom="4.391928094887362" center=[128.1361269438078,-31.53688018319827] animationOptions={duration:500}}-->
#### 09 November 2019
Explore more dates on the [Dashboard](https://eodashboard.org/explore?x=14264048.40361&y=-3702671.30498&z=4.39193&indicator=N1_CO)


## <!--{ as="div" }--> Open Science
### Open Science
All datasets referenced in this story are freely and openly available. 

| Name | Type | Agency / Provider | Description | Access |
|---|---|---|---|---|
| [Copernicus Sentinel-5P TROPOMI - Carbon Monoxide (CO)](https://eodashboard.org/explore?indicator=N1_CO) | Dataset | ESA / Copernicus | Daily atmospheric column CO concentrations derived from TROPOMI; used as proxy to estimate CO2 emissions from the 2019–2020 Australian bushfires | [EO Dashboard](https://eodashboard.org/explore?indicator=N1_CO) |
| [Copernicus Sentinel-5P TROPOMI - Nitrogen Dioxide (NO2)](https://eodashboard.org/explore?indicator=N1_NO2) | Dataset | ESA / Copernicus | Daily atmospheric column NO2 concentrations derived from TROPOMI; global coverage | [EO Dashboard](https://eodashboard.org/explore?indicator=N1_NO2) |
| [Copernicus Sentinel-5P TROPOMI - Sulfur Dioxide (SO2)](https://eodashboard.org/explore?indicator=N1_SO2) | Dataset | ESA / Copernicus | Daily atmospheric column SO2 concentrations derived from TROPOMI; global coverage | [EO Dashboard](https://eodashboard.org/explore?indicator=N1_SO2) |
| [Copernicus Sentinel-5P Mission](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-5p) | Mission | ESA / Copernicus | First Copernicus mission dedicated to atmospheric monitoring; carries the TROPOMI instrument measuring trace gases including CO, NO2, SO2, CH4, O3, and aerosols | [ESA Sentinel Online](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-5p) |
| [EO Dashboard](https://eodashboard.org/explore) | Platform | ESA / NASA / JAXA | Trilateral open Earth observation dashboard providing interactive maps of TROPOMI trace gas datasets and other EO products | [eodashboard.org](https://eodashboard.org/explore) |


