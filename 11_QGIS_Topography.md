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

Download a set of GeoTIFFs from a website of your choice. This tutorial will focus on the Klopstockwiese in Zurich. ([Zurich GIS](https://maps.zh.ch/))
Since larger datasets are usually divided into smaller tiles the download of the selected area as shown in the picture below will likely contain several tiles. In this case your download will include four .tif files.


![QGIS_ZH_GIS](/doc/QGIS_ZH_GIS.jpg)

---

After downloading the different tiles they have to be unpacked and afterwards combined into one consistent raster file. For this step we are only interested in the .tif file from the download folder. Drag and drop those files into your QGIS workspace to load them. They are currently not connected and have their own colour range indication the height of that raster point. The breaks between the different sets are clearly visible.

![QGIS_LoadDOM_DTM](/doc/QGIS_LoadDOM_DTM.jpg)

---
## Merging Raster Layers  

To combine the different tiles go to Raster > Miscellaneous > Merge

![QGIS_LoadDOM_DTM](/doc/QGIS_CombineDOM_DTM.jpg)

Select the raster sets you would like to combine by clicking on the three dots in the top right corner (see image below). 

![QGIS_LoadDOM_DTM_II](/doc/QGIS_CombineIIDOM_DTM.jpg)

In this case you can select all of them. Press "Run" after selecting the raster sets.

![QGIS_LoadDOM_DTM_III](/doc/QGIS_CombineIIIDOM_DTM.jpg)

---

## Correcting the raster values

After merging you might notice that the values of the new file are not the same as in the original files (compare the maximum and minimum raster values). This inconvenience can be solved by adjusting the layer properties. Select the merged raster layer, right-click on it and navigate to "Layer Properties".

![QGIS_LayerProperties](/doc/QGIS_LayerProperties.jpg)

Whithin the properties window navigate to "Symbology" and expand the "Min / Max Value Settings" tab by clicking on it (see image below).

![QGIS_LayerProperties_II](/doc/QGIS_LayerPropertiesII.jpg)

Within the Min / Max Value Settings change the accuracy from "Estimate (faster)" to "Actual (slower)". Click apply and close the properties window. Now the values should the same as your input layers.

![QGIS_LayerProperties_II](/doc/QGIS_LayerPropertiesIII.jpg)

---

## Clipping the Raster Layer

To limit the raster layer to the area we are interested in select the merged raster layer and go to Raster > Extraction > Clip Raster by Extend. Make sure the merged raster layer is selected at the top. For the field "Lcuping Extend" choose "Draw on Canvas". Alternatively you could also use a preset rectangular shapefile as a clipping boundary. Click "Run" and close the window. 


![QGIS_LayerClipping](/doc/QGIS_ClippingLayer.jpg)

After disabling the merged layer the clipped extend might look somewhat like this:

![QGIS_LayerClippingII](/doc/QGIS_ClippingLayerII.jpg)

---

## Raster to Point

To turn our raster data into a point set which we can import and open in Rhinoceros 3D we have to use the Processing Toolbox. To open the toolbox panel go to Processing > Toolbox. The toolbox offers a wide range of geoprocessing tools and has a surprisingly good search function.

![QGIS_Toolbox](/doc/QGIS_Toolbox.jpg)

The tool we need is called "Raster values to points"

![QGIS_Toolbox](/doc/QGIS_ToolboxII.jpg)



## Setup

![RhinoCam_Setup_1](/doc/RhinoCam_Setup_1.png)

>##### Setup Document:
>1. Verify Units: go to Options > Units: make sure the document-units are set to millimeters When you create a new document: select Small Objects - Millimeters
