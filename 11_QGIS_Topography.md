# QGIS From DTM / DSM to Topography

This tutorial will illustrate the process of importing and transforming Digital Terrain Models (DTM) or Digital Surface Models (DSM) into a .xyz or .csv file for further manipulation.
DTMs and DSMs are commonly provided by municipalities as base data for planning tasks. However they usually come in the format GeoTIFF, a geo-located picture format, that is incompatible with most CAD programs. To transform the file into a usable three-dimensional topography model, several transformation steps have to be undertaken in QGIS. These steps will be illustrated in the following. 

---

## Content
*Jump to the topic you are looking for*

- [RhinoCam Workflow](#rhinoCam-workflow)
- [Setup](#setup)
- [Tools](#tools)
- [Machining Operations](#machining-operations)
- [Regions & Curves](#regions-and-curves)
- [Post Processing](#post-processing)

---

## Importing DTM / DSM to QGIS  

Download a set of GeoTIFFs from a website of you choice. This tutorial will focus on the Klopstockwiese in Zurich. ([Zurich GIS](https://maps.zh.ch/))
Since larger datasets are usually divided into smaller tiles the download of the selected area as shown in the picture below will likely contain several tiles. In this case your download will include four .tif files.


![QGIS_ZH_GIS](/doc/QGIS_ZH_GIS.jpg)

---

After downloading the different tiles they have to be unpacked and afterwards combined into one consistent raster file. For this step we are only interested in the .tif file from the download folder. Drag and drop those files into your QGIS workspace to load them. They are currently not connected and have their own colour range indication the height of that raster point. The breaks between the different sets are clearly visible.

![QGIS_LoadDOM_DTM](/doc/QGIS_LoadDOM_DTM.jpg)

---

To combine the different tiles go to Raster > Miscellaneous > Merge

![QGIS_LoadDOM_DTM](/doc/QGIS_CombineDOM_DTM.jpg)

Select the raster sets you would like to combine by clicking on the three dots in the top right corner (see image below). 

![QGIS_LoadDOM_DTM](/doc/QGIS_CombineIIDOM_DTM.jpg)

In this case you can select all of them. Press "Run" after selecting the raster sets.

![QGIS_LoadDOM_DTM](/doc/QGIS_CombineIIIDOM_DTM.jpg)

---



## Setup

![RhinoCam_Setup_1](/doc/RhinoCam_Setup_1.png)

>##### Setup Document:
>1. Verify Units: go to Options > Units: make sure the document-units are set to millimeters When you create a new document: select Small Objects - Millimeters
