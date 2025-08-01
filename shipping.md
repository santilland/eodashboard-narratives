---
cover-image: https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/12-ship-traffic.jpg
date: 2025-01-01
theme: covid-19
tags: shipping
official: true
---

#  Travel restrictions interrupted Global Supply chains dependent on cargo shipping<!--{ as="img" mode="hero" src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/12-ship-traffic.jpg" }-->
### Covid-19 Impacts on global shipping, observed from satellites<!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->

## Satellite observations of supply chains

Supply chains around the world dependent on cargo shipping have been interrupted by travel restrictions and quarantines designed to stop the spread of the novel coronavirus. Many ports are closed, shipments have been canceled, and, in some locations, altered shipping routes have prevented the efficient movement of cargo.

NASA and ESA researchers are using cutting-edge artificial intelligence technology and high-resolution satellite imagery from [Planet Labs](https://www.planet.com/) and [Sentinel-2](https://sentinel.esa.int/web/sentinel/missions/sentinel-2) to track shipping activity at major ports in the U.S. and in Europe during the coronavirus pandemic.

This data will help quantify the level of shipping-related economic activity over time and could eventually contribute to our understanding of the environmental implications of global decreases in shipping on key air pollutants like nitrogen dioxide (NO<sub>2</sub>) and sulphur dioxide (SO<sub>2</sub>).

### Detection of ships on PlanetScope images

NASA’s Interagency Implementation and Advanced Concepts Team (IMPACT), based at NASA’s Marshall Space Flight Center in Huntsville, Alabama, trained an algorithm using supervised machine learning technique to detect ships on PlanetScope images. The algorithm detects a ship on the image and geolocates it. The NASA team has also built an Application Programming Interface (API) that allows ship detections to be aggregated across a port area for a given day. Efforts are also underway to conduct a study of ship detections in U.S. ports during the period of pandemic travel restrictions, as compared to the same period of time in previous years.

NASA researchers have access to the high-resolution imagery from Planet Labs, through the Commercial SmallSat Data Acquisition Program (CSDAP), which acquires data from commercial sources that support NASA's Earth science research goals. The PlanetScope image resolution is 3 meters per pixel, which allows researchers to get a detailed look at changes occurring on the ground. Commercial small satellites also provide high temporal resolution, making images available almost every day (depending on cloud cover) for key areas of interest.

Ship detections can be provided daily, except when prevented by significant cloud cover. After the machine learning model detects the ships, a secondary human validation is also performed before the detections are made available for the dashboard.

Learn more about the NASA research using AI on Planetscope imagery from the [NASA VEDA Dashboard](https://www.earthdata.nasa.gov/dashboard/stories/changing-landscapes).


## Ship Detections in Sentinel-2 imagery

ESA engineers based at ESA's [Centre for Earth Observation (ESRIN)](https://www.esa.int/About_Us/ESRIN) trained a Machine Learning algorithm to recognise ships on Copernicus Sentinel-2 satellite images. Sentinel-2 provides high-resolution (10 meters) multi-spectral imagery for land services. It provides for example, imagery of vegetation, soil and water cover, inland waterways and coastal areas. Sentinel-2 also delivers information for emergency services. The Copernicus Sentinel-2 mission comprises a constellation of two polar-orbiting satellites and has a high revisit time (10 days at the equator with one satellite, and 5 days with 2 satellites under cloud-free conditions which results in 2-3 days at mid-latitudes).

To reduce the number of false alarms and mis-detections, a cloud-masking operation is performed on the images before the Machine Learning algorithm is applied. The outputs of the Machine Learning algorithm are bounding boxes of the detected ships within pre-defined areas of interest at major European harbours, such as Genova in Italy or Hamburg in Germany.

## Port of Genoa<!--{ as="eox-map" mode="tour" }-->

### <!--{ layers='[{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"IT3;:;2019-03-23T10:38:25;:;E13c_shipping_activity;:;EPSG:3857","title":"E13c_shipping_activity"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["SENTINEL-2-L2A-TRUE-COLOR"],"TILED":true,"TIME":"2019-03-23T10:38:25/2019-03-23T22:38:24"}}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"osm","title":"Background"},"source":{"type":"OSM"}}]}]' zoom="14.55627077678812" center=[8.906844181890747,44.40546025815988] projection="" animationOptions={duration:500}}-->
#### Copernicus Sentinel-2 
#### Port of Genoa, Italy

observation date: **23 March 2019**

### <!--{ layers='[{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"IT3;:;2020-03-22T10:28:28;:;E13c_shipping_activity;:;EPSG:3857","title":"E13c_shipping_activity"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["SENTINEL-2-L2A-TRUE-COLOR"],"TILED":true,"TIME":"2020-03-22T10:28:28/2020-03-22T22:28:27"}}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"osm","title":"Background"},"source":{"type":"OSM"}}]}]' zoom="14.55627077678812" center=[8.906844181890747,44.40546025815988] projection="" animationOptions={duration:500}}-->
#### Copernicus Sentinel-2 
#### Port of Genoa, Italy

observation date: **22 March 2020**
The reduced activity in the port is observed compared to the same date in the previous and successive years. 


### <!--{ layers='[{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"IT3;:;2021-03-22T10:28:31;:;E13c_shipping_activity;:;EPSG:3857","title":"E13c_shipping_activity"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["SENTINEL-2-L2A-TRUE-COLOR"],"TILED":true,"TIME":"2021-03-22T10:28:31/2021-03-22T22:28:30"}}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"osm","title":"Background"},"source":{"type":"OSM"}}]}]' zoom="14.55627077678812" center=[8.906844181890747,44.40546025815988] projection="" animationOptions={duration:500}}-->
#### Copernicus Sentinel-2 
#### Port of Genoa, Italy

observation date: **22 March 2021**


