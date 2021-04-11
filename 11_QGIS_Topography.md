# QGIS From DTM / DSM to Topography

This tutorial will illustrate the process of importing and tranforming a Digital Terrain Model (DTM) or Digital Surface Model (DSM) into a .xyz or .csv file for further manipulation.
DTMs and DSMs are commonly provided by municipalities as base data for planning tasks. However they usually come in the format GeoTIFF, a geo-located picture format, that is incompatible with most CAD programs. To transform the file into a three-dimensional topography model, several transformation steps have to be undertaken in QGIS. These steps will be illustrated in the following. 

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

## Importing DTM /DSM to QGIS  

>Download a set of GeoTIFFs from a website of you choice. This tutorial will focus on the Klopstockwiese in Zurich. ([Zurich GIS](https://maps.zh.ch/))
>Since larger datasets are usually divided into smaller tiles the download of the selected area as shown in the picture below will likely contain several tiles. In this case your download will include four .tif files.
>

![QGIS_ZH_GIS](/doc/QGIS_ZH_GIS.jpg)

>After downloading the different tiles they have to be unpacked and afterwards combined into one consistent raster file. For this step we are only interested in the .tif file from the download folder. Drag and drop those files into your QGIS workspace to load them.  
>

![QGIS_LoadDOM_DTM](/doc/QGIS_LoadDOM_DTM.jpg)

---

## Setup

![RhinoCam_Setup_1](/doc/RhinoCam_Setup_1.png)

>##### Setup Document:
>1. Verify Units: go to Options > Units: make sure the document-units are set to millimeters When you create a new document: select Small Objects - Millimeters
