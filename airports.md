---
cover-image: https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/trilateral/Esa_Nasa_jaxa_covid19_cover_V3.jpg
date: 2025-01-01
theme: covid-19
tags: travel,airplane,lockdown
official: true
---

#  During COVID-19 related lockdowns, air travel decreased<!--{ as="img" mode="hero" src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/trilateral/Esa_Nasa_jaxa_covid19_cover_V3.jpg" }-->
### How EO and AI can illustrate COVID-19 impacts on air travel<!--{ style="font-size:1.5rem;opacity:0.7;margin-top:1rem;" }-->

## Grounded airplanes during COVID-19 pandemic

During COVID-19 related lockdowns, activities like air travel decreased to prevent the spread of the novel coronavirus. To help quantify these changes, scientists are combining two kinds of space-based remote sensing data – synthetic aperture radar (SAR) data from JAXA’s ALOS-2 and [ESA’s Copernicus Sentinel-1](https://sentinel.esa.int/web/sentinel/missions/sentinel-1) satellites with NASA-processed high-resolution optical remote sensing data from Planet Inc. and [ESA's Copernicus Sentinel-2 multispectral satellite data](https://sentinel.esa.int/web/sentinel/missions/sentinel-2) – to observe and quantify the changes in grounded airplanes and air traffic around the world.

SAR is a high-resolution, space-based radar that makes 2D images out of 3D objects. By comparing SAR images of airports before, during, and after lockdowns, scientists can determine how air traffic may have changed during the pandemic. In general, manmade targets such as buildings, cars, and airplanes appear brighter in SAR imagery than natural targets like bare land, forested areas, or the ocean.

Figure 1. shows a color composited SAR image of Tokyo International Airport, Haneda from the PALSAR-2 instrument aboard the ALOS-2 satellite. The different colors in the image correspond to the different dates the images were captured: red images were captured before lockdowns on November 28, 2019, green images were captured as lockdowns began on March 19, 2020, and blue images were captured during lockdowns on May 14, 2020. White colored areas, such as buildings, indicate no changes during the time period, whereas individual red, green, or blue colored pixels in the parking areas of the airport indicate airplanes at that time. Cyan colored areas show airplanes on March and May 2020.

Figure 2 shows a time series animation of SAR images taken from [Sentinel-1](https://sentinel.esa.int/web/sentinel/missions/sentinel-1) at Tokyo International Airport, Haneda from January 10 to June 2, 2020. Brighter pixels in parking areas of the airport may correspond with airplanes at each acquisition date.

<center>
<figure>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/trilateral/JP01-E8_Fig1.png" alt="PALSAR-2 Tokyo Airport">
  <figcaption>Figure 1. A multi-temporal, color-composite PALSAR-2 image at Tokyo International Airport, Haneda acquired on November 2019 (red), March 2020 (green), and May 2020 (blue).</figcaption>
</figure>

<center>
<figure>
  <img src="https://raw.githubusercontent.com/eurodatacube/eodash/c59adc7d580c6ced1f85a44c5bdd18bf94b3c9ee/app/public/data/trilateral/JP01-E13b_Animation.gif" alt="PALSAR-2 Tokyo Airport">
  <figcaption>Figure 2. Sentinel-1 animation at Tokyo International Airport, Haneda from January to June 2020. Brighter pixels in parking areas of the airport may correspond with airplanes at each acquisition date</figcaption>
</figure>
</center>
	
## 

In addition to the SAR imagery, NASA and ESA scientists also used artificial intelligence technology and high-resolution optical imagery from Planet and [Copernicus Sentinel-2](https://sentinel.esa.int/web/sentinel/missions/sentinel-2) to detect and count aircraft on the ground at airports.

Combining high-resolution optical remote sensing data from Planet and Sentinel-2 with SAR imagery from ALOS-2 and [Sentinel-1](https://sentinel.esa.int/web/sentinel/missions/sentinel-1) is a powerful method to provide reliable time series data on the number of aircrafts grounded at airports over time. While imagery from optical satellites like Planet or [Sentinel-2](https://sentinel.esa.int/web/sentinel/missions/sentinel-2) is powerful to monitor changes in grounded aircrafts around the world systematically, their sensors cannot penetrate clouds, limiting the detection capability on cloudy or rainy days. Alternatively, SAR data, while lower resolution, can penetrate clouds. Therefore, scientists are combining these datasets to get the most comprehensive images of changes at aircraft counts at airports during the COVID-19 pandemic.

## Paris Airport (CDG) <!--{ as="eox-map" mode="tour" }-->
### <!--{ layers='[{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"FR8;:;2019-04-21T11:11:06;:;E13b_parked_airplanes;:;EPSG:3857","title":"E13b_parked_airplanes"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["SENTINEL-2-L2A-TRUE-COLOR"],"TILED":true,"TIME":"2019-04-21T11:11:06/2019-04-21T23:11:05"}}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"osm","title":"Background"},"source":{"type":"OSM"}}]}]' zoom="14.292591536229368" center=[2.57512311456145,49.00363044105609] projection="" animationOptions={duration:500}}-->
#### Copernicus Sentinel-2 observations 
#### Paris Airport Charles de Gaule

observation date: **21 April 2019**

### <!--{ layers='[{"type":"Group","properties":{"id":"AnalysisGroup","title":"Data Layers"},"layers":[{"type":"Tile","properties":{"id":"FR8;:;2020-04-25T10:57:23;:;E13b_parked_airplanes;:;EPSG:3857","title":"E13b_parked_airplanes"},"source":{"type":"TileWMS","url":"https://services.sentinel-hub.com/ogc/wms/0635c213-17a1-48ee-aef7-9d1731695a54","projection":"EPSG:4326","tileGrid":{"tileSize":[512,512]},"params":{"LAYERS":["SENTINEL-2-L2A-TRUE-COLOR"],"TILED":true,"TIME":"2020-04-25T10:57:23/2020-04-25T22:57:22"}}}]},{"type":"Group","properties":{"id":"BaseLayersGroup","title":"Base Layers"},"layers":[{"type":"Tile","properties":{"id":"osm","title":"Background"},"source":{"type":"OSM"}}]}]' zoom="14.292591536229368" center=[2.57512311456145,49.00363044105609] projection="" animationOptions={duration:500}}-->
#### Copernicus Sentinel-2
#### Paris Airport Charles de Gaule

observation date: **25 April 2020**

The COVID-19 pandemic has resulted in airlines temporarily grounding large numbers of aircrafts. These observations from Copernicus Sentinel-2 capture the differences between the number of parked planes at approximately the same date in April 2019 (before the pandemic) and 2020 (at the peak of the pandemic restrictions). 

This chart shows the variation in the detected number of parked airplanes at CDG Airport using Sentinel-2 imagery and AI.
	
![](https://raw.githubusercontent.com/aapopescu/eodashboard-narratives/aapopescu/corrections-stories-before-lps/assets/aapopescu/CDG-parked-planes-1750505646482.png)

Further dates can be explored on the [Dashboard](https://eodashboard.org/explore/?x=2.5751&y=49.0036&z=14.2926&datetime=2020-04-25&template=expert&indicator=E13b&poi=FR8).

