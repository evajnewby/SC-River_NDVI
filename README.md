# Santa Clara River Plant Phenology

Author: Eva Newby (https://github.com/evajnewby)

## About
The following repository was created for edicational purposes for EDS 220 - Environmental Data, for the Masters of Environmental Data Science program at the Bren School of Environmental Science and Management at the University of California, Santa Barbara. 

The purpose of this repository is to hold both data and code necessary for the completion of the Normalized Difference Vegetation Index (NDVI) maps and one plot showing the seasonal cycles of vgetation productivity compared with the NDVI for the Santa Clara River. 

This repository contains one data folder, one R project, one Quarto document, one rendered html and associated files. 

The `SC_River_NDVI.qmd` contains all the code necessay to read in the raster data, make an NDVI function, compute NDVI for all scenes, and compare NDVI across vegetation communities. The `SC_River_NDVI.html` is the rendered version. 

The data folder contains the landsat data tif files for the dates, along with the study_sites.shp, .prj, and .dbf. This folder was added to the gitignore to prevent any pushing issues or delays.

## Highlights
-   Compare seasonal patterns across the aforementioned vegetation communities
-   Calculate NDVI
-   Visualize NDVI changes within the riparian, grassland, and chaparral vegetation communities.

## Data
The data contains multi-spectral remote sensing data from the Landsat's operational land imager with 8 pre-processed scenes:
- Level 2 surface reflectance products,
- Erroneous values set to NA,
- Scale factor set to 100,
- Bands 2-7,

Dates in file name with scenes from the following dates:
- 2018-06-12,
- 2018-08-15,
- 2018-10-18,
- 2018-11-03,
- 2019-01-22,
- 2019-02-23,
- 2019-04-12,
- 2019-07-01.
  
Additionally, the study_sites.shp are polygons representing the vegetation community sites.

## Repository Structure
```bash
SC-River-NDVI
├── README.md
├── .gitignore
      ├── data
          ├── landsat_20180612.tif
          ├── landsat_20180815.tif
          ├── landsat_20181018.tif
          ├── landsat_20181103.tif
          ├── landsat_20190122.tif
          ├── landsat_20190223.tif
          ├── landsat_2010412.tif
          ├── landsat_20190701.tif
          ├── study_sites.prj
          ├── study_sites.dbf
          ├── study_sites.shp
          ├── study_sites.shx
├── SC_River_NDVI.Rproj
├── SC_River_NDVI_files
├── SC_River_NDVI.html
└──  SC_River_NDVI.qmd
```

## References
Data citation: NASA. Operational Land Imager (OLI) on Landsat 8. NASA's Landsat Missions. Retrieved December 5, 2024, from https://landsat.gsfc.nasa.gov/satellites/landsat-8/spacecraft-instruments/operational-land-imager/
