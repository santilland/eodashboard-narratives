---
cover-image: https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/CryoSat.jpeg
date: 2025-01-01
theme: cryosphere
tags: climate,ice,polar,warming
official: true
---

#   Measuring Thickness of Sea Ice in the Polar Oceans<!--{ as="img" mode="hero" src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/story-images/CryoSat.jpeg" }-->
### Read more about monitoring Sea Ice Freeboard & Thickness from Satellite Altimetry. <!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->

## Sea Ice Freeboard and Thickness

NASA provides data collected over the Arctic Ocean by the Ice, Cloud and land Elevation Satellite-2 (ICESat-2) that show monthly sea ice freeboard from 2018 to the present. Sea ice freeboard is the amount of sea ice and snow cover that is visible above the surface of the ocean and, along with snow depth, is a critical measurement for accurately measuring the thickness of sea ice in the polar oceans. Click [here](https://icesat-2.gsfc.nasa.gov/science) to learn more about this research.

NASA’s ICESat-2 mission has been measuring the height of the Earth’s features from space with a laser ever since its launch in September 2018. The Advanced Topographic Laser Altimeter System (ATLAS) onboard ICESat-2 shoots pulses of light towards the Earth’s surface. ATLAS counts the particles of light (i.e., photons) that bounce off the Earth’s surface and return to the instrument’s sensors, measuring the round-trip time of each photon with extreme accuracy. Scientists can then take the total elapsed time to generate a height measurement of the particular surface that each photon bounced from. When enough photon measurements have been collected, scientists clump these measurements together to form a “photon cloud” that produces continuous surface elevation measurements as the satellite collects more and more data along its orbit. ICESat-2 collects data over the same location every 91 days, and this allows scientists to develop a picture of how the heights at certain spots around the globe are changing over time.

Collecting repeated height measurements of the Earth’s ice from space is an important way to view changes happening over the course of seasons and years. While ICESat-2 can only measure the height of Earth’s ice, scientists utilize special formulas (based on Archimedes' principle) to take those height measurements and turn them into measurements of sea ice freeboard that includes the ice above and below the waterline.

## ICESat-2 Map <!--{ as="eox-map" mode="tour" }-->
### <!--{ layers='[{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857"}}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"SITI_IS2SITMOGR4-cog;:;IS2SITMOGR4_01_202104_005_002;:;SITI_IS2SITMOGR4-cog;:;EPSG:3857","title":"SITI_IS2SITMOGR4-cog"},"source":{"type":"XYZ","url":"https://openveda.cloud/api/raster/cog/tiles/WebMercatorQuad/{z}/{x}/{y}?url=s3://veda-data-store/IS2SITMOGR4-cog/IS2SITMOGR4_01_202104_005_002.tif&resampling_method=nearest&bidx=1&colormap_name=plasma&rescale=0.0,4.0","projection":"EPSG:3857"}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"cloudless-2023;:;EPSG:3857","title":"EOxCloudless 2023"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2023_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"},"visible":true},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"},"visible":false},{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"},"visible":false}]}]' zoom="2.549999887817721" center=[-93.09001748296997,67.57198410167112] projection="" animationOptions={duration:500}}-->
#### Sea Ice Thickness (ICESat-2)
observation date: **30 April 2021**

This data set reports monthly, gridded winter sea ice thickness across the Arctic Ocean. Sea ice thickness is estimated using ATLAS/ICESat-2 L3A Sea Ice Freeboard (ATL10), Version 5 data and NASA Eulerian Snow On Sea Ice Model (NESOSIM) snow loading.

Explore more dates on the [Dashboard](https://eodashboard.org/explore/?x=-35.2414&y=67.5448&z=2.5488&datetime=2021-04-30&template=expert&indicator=SITI)

## ESA's CryoSat-2 & Envisat

While measurements from ICESat-2 can be used to determine the height and freeboard of polar sea ice, scientists also rely on ESA and the CryoSat-2 mission to measure sea ice thickness. Researchers at ESA provide monthly measurements of sea ice thickness from the CryoSat-2 and Envisat radar altimeters and other supporting missions.

Watch this video to learn how ESA measures sea ice thickness from space.

<iframe width="560" height="315" src="https://www.youtube.com/embed/9einyMSOmHE?si=Sj-70Ym8hiDPkpi_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Explore Datasets

This **EO Dashboard** provides access to interactive maps of Sea Ice Thickness and Sea Ice Concentration. Access these datasets directly from the links below:

- [Sea Ice Thickness from Cryosat](https://eodashboard.org/explore?indicator=SIC)
- [Sea Ice Thickness from Envisat](https://eodashboard.org/explore?indicator=SIE)
- [Sea Ice Thickness from IceSAT-2](https://eodashboard.org/explore?indicator=SITI)
- [Sea Ice Concentration Antarctic from GCOM-W](https://eodashboard.org/explore?indicator=World-N12_1_sea_ice_concentration_arctic)








## ENVISAT Map<!--{ as="eox-map" mode="tour" }-->

### <!--{ layers='[{"type":"Group","properties":{"id":"OverlayGroup","title":"Overlay Layers"},"layers":[{"type":"Tile","properties":{"id":"overlay_bright;:;EPSG:3857","title":"Overlay labels"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/overlay_base_bright_3857/default/g/{z}/{y}/{x}.png","projection":"EPSG:3857"}}]},{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"sea_ice_thickness_envisat;:;22358;:;sea_ice_thickness_envisat;:;EPSG:3857","title":"sea_ice_thickness_envisat"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["ESA-CCI-V2-ENVISAT"],"TILED":true,"TIME":"2012-03-01T00:00:00Z/2012-03-01T23:59:59Z"}}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"cloudless-2023;:;EPSG:3857","title":"EOxCloudless 2023"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/s2cloudless-2023_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"},"visible":true},{"type":"Tile","properties":{"id":"OSM;:;EPSG:3857","title":"OSM Background"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/osm_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"},"visible":false},{"type":"Tile","properties":{"id":"terrain-light;:;EPSG:3857","title":"Terrain Light"},"source":{"type":"XYZ","url":"//s2maps-tiles.eu/wmts/1.0.0/terrain-light_3857/default/g/{z}/{y}/{x}.jpeg","projection":"EPSG:3857"},"visible":false}]}]' zoom="2.548821908458751" center=[-70.02618074098795,61.83987169126752] projection="" animationOptions={duration:500}}-->
#### Envisat Sea Ice Thickness Product

observation date: **01 March 2012**

This dataset provides a Climate Data Record of Sea Ice Thickness for the northern hemisphere polar region, derived from the RA-2 (Radar Altimeter -2) instrument on the  satellite. This product was generated in the context of the ESA Climate Change Initiative Programme () by the Sea Ice CCI () project.

It provides daily sea ice thickness data for the winter months of October to April annually on the satellite measurement grid (Level 2P) at the full sensor resolution for the period October 2002 to March 2012.

Explore more dates on the [Dashboard](https://eodashboard.org/explore/?x=-70.0262&y=61.8399&z=2.5488&datetime=2012-03-01&template=expert&indicator=SIE)
