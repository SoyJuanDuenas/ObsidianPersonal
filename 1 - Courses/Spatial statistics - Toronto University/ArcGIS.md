#spatial 

ArcGIS is a comprehensive [[Geographical Information Systems (GIS)]] platform developed by Esri (Environmental Systems Research Institute). It provides tools and capabilities for mapping, [[spatial analysis]], data management, and geospatial data visualization. ArcGIS is widely used across various industries, including urban planning, environmental science, transportation, public health, and more.

_Components of ArcGIS_

1. **ArcGIS Desktop**:
    
    - **ArcMap**: A traditional GIS application for creating maps, performing [[spatial analysis]], and managing [[geospatial data]]. It allows users to work with both [[vector data]] and [[raster data]], perform complex [[geoprocessing task]], and create detailed cartographic outputs.
    - **ArcCatalog**: A file management tool integrated within ArcGIS Desktop that helps users organize, browse, and manage spatial datasets and metadata.
    
2. **ArcGIS Pro**: 
	- A more modern, 64-bit GIS application designed for advanced visualization, 3D analysis, and the integration of data from multiple sources. ArcGIS Pro is gradually replacing ArcMap as the primary desktop GIS tool in the ArcGIS suite.

# A little overview

in Data view se can see our [[map]], the table of contents list all maps and layers we're using currently, the table is the dataset associated to the layer we select, in Catalog we see ArcCatalog that allow us to make file management. finally in ArcToolBox we can find folders that holds different task we can perform to edit, convert and analyze our data. 

![[Pasted image 20240803164555.png]]

In ArcCatalog we can preview the data and read metadata (information about the dataset)

# Types of files 

## .mxd

This type of file called Map Document store What data to show (select), Where to find the data (rute), How show the data (appearance) but it does not store the actual map data. If the software cannot open the location where the data are stored, then will pop up a red exclamation mark.

A way to make sure that doesn't happen is using relative paths this can be done in customize/General/Make relative paths the default for new map documents.

## .mpk

Packages a map document and all referenced data sources to create a single compressed .mpk file

## .lyr

This type of file called Layer File store what data are going to be used and also how show that data, but just for one feature class. So it is useful to save the symbiology of that layer associated to a rute where are store some data. (this do not save the data) if we want to save a copy of the data we should use the option of *export the data*.

