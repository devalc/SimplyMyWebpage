---
author: Chinmay Deval
categories:
- Geoserver
- OpenLayers
- JavaScript

date: "2023-05-16"
draft: false
excerpt: Using historic satellite remote sensing evapotranspiration imagery this tool helps identify fields that could potentially benefit from variable rate management strategies.
featured: true
layout: single
links:
- icon: door-open
  icon_pack: fas
  name: application website
  url: https://devalc.github.io/ETPersistence/
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/devalc/ETPersistence
subtitle: ""
tags:
- hugo-site
title: ET-Persistance
subtitle: (Note- This tool is currently supported only in Mozilla Firefox browser.)
---
The ET Persistence layers are available to visualize online using Mozilla Firefox browser at:  [ET-Persistence](https://devalc.github.io/ETPersistence/)

<p align="center">
  <img src="ET_featured.PNG">
</p>


## Features

- Online Visualization Tool: [ET-Persistence](https://devalc.github.io/ETPersistence/)
- Seamless integration of ET Persistence WMS Layer into QGIS.
- Access to valuable ET Persistence data for informed decision-making.
- Easy visualization of ET Persistence information within GIS projects.

## Installation

There is no specific installation required for this repository. The integration process involves configuring the ET Persistence WMS Layer in your GIS software. Please refer to the usage instructions below for more details.

## Usage

To add the ET Persistence WMS Layer to QGIS, follow these steps:

1. Open QGIS and navigate to the "Layer" menu.
2. Select "Add Layer" > "Add WMS/WMTS Layer".
3. In the "Data Source Manager" window, click on the "New" button to create a new connection to the WMS service.
4. Enter a name for the connection.
5. Enter the following WMS server URL: [http://dev.wepp.cloud:1337/geoserver/magicvalley/wms?](http://dev.wepp.cloud:1337/geoserver/magicvalley/wms?)
6. Click "OK" and then click "Connect" to retrieve the available layers from the WMS service.
7. Select the desired ET Persistence layer.
8. Click "Add" to incorporate the layer into your QGIS project.

## Description
Many growers now have the ability to adopt variable rate management strategies to optimize crop performance and profitability within a specific field. But targeting those managements is challenging. Using historic satellite remote sensing evapotranspiration imagery this tool helps identify fields that could potentially benefit from variable rate management strategies. It provides pre-processed interactive maps that show the proportion of the field which either consistently under-performs or over-performs relative to the field average.

We used historic 30 m gridded seasonal consumptive irrigation requirement maps (i.e. actual evapotranspiration or crop water uptake) developed by the University of Idaho and the Idaho Department of Water Resources over an 11 year period to identify fields that demonstrate consistent crop performance patterns. Each year we calculated relative crop water use for each pixel (relative to the field mean). A value of 1 indicates the specific point in a field responds similarly to the average for the entire field.  Hypothesis testing using this relative crop water use maps for each pixel in the field we determine whether the relative crop water use over the 11 years was statistically different than the field average at a 95% confidence interval.  

In some cases, a grower might be more conservative and would like to define a portion of a field as performing persistently different based on a specific threshold. To address this concern we also created maps the identified the portion of a field where the relative crop water use was greater than 5% different than the field average.