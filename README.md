# Mapping the 2025 Eaton and Palisades Wildfires in Los Angeles County and Social Impacts
# Author: Marie Tolteca
# Date: 12/12/2025

## About:
This repository contains code and materials for analyzing Landsat imagery and mapping wildfire perimeters in Los Angeles County. It demonstrates how to:
- Work with NetCDF (.nc) Landsat data
- Read and reproject shapefiles
- Create true-color (RGB) and false-color composites
- Overlay geospatial data to visualize fire boundaries
- Generate publication-quality figures
- Develop clear and reproducible geospatial workflows

The focus is on the Eaton and Palisades Fires, combining satellite imagery with official fire perimeter shapefiles to explore fire-affected areas.

Satellite imagery shows the Eaton and Palisades wildfires in Los Angeles County (NPR, 2025).

<img width="1200" height="630" alt="image" src="https://github.com/user-attachments/assets/ef4526e9-3516-44e5-881a-13693b844133" />

# Data
- The Landsat .nc file can be downloaded from a shared Google Drive folder provided by the instructor for the course EDS 220 – Working with Environmental Datasets:
[Google Drive Link](https://drive.google.com/drive/folders/1USqhiMLyN8GE05B8WJmHabviJGnmAsLP)
- Fire perimeter shapefiles for the Palisades and Eaton fires were obtained from the County of Los Angeles GIS:
County [GIS Link](https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about)
- Each shapefile contains a dissolved fire perimeter for its respective fire and has been added to the data folder in this repository.

## Repository Structure:
- **When downloading data, add the data folder to `.gitignore` to reduce pushing big files onto github.**
```
├── la_wildifre_and_social_impacts.ipynb
├── README.md
└── data
    ├── landsat8-2025-02-23-palisades-eaton.nc
    ├── Palisades_Perimeter_20250121.shp
    │   └── palisades_perimeter.md
    └── Eaton_Perimeter_20250121.shp
        └── eaton_perimeter.md
    └── EJI_2024_California
        └── EJI_2024_California.gdb
```
# Packages Used:
This notebook uses the following Python packages: `os`, `numpy`, `matplotlib.pyplot`,  `matplotlib.patches`,`geopandas`, `xarray`, and `rioxarray`.

# Highlights:
- Data exploration of Landsat imagery and shapefiles
- Restoration of geospatial information (CRS)
- True-color and false-color visualization
- Overlay of Eaton and Palisades fire perimeters on false-color composite
- Creation of publication-quality figures

#### References:
- Assignment 4: Palisades & Eaton Fires. EDS 220 – Working with Environmental Datasets, 2025. https://meds-eds-220.github.io/EDS-eds-220-course/assignments/assignment4-palisades-eaton-fires.html. Accessed 17 Nov. 2025.
- Microsoft Planetary Computer. Planetary Computer. (n.d.). https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2
- NPR. Satellite image ©2025 Maxar Technologies (January 9, 2025). https://www.kpbs.org/news/national/2025/01/09/photos-see-the-california-wildfires-destructive-force-in-satellite-images
- Palisades and Eaton dissolved fire perimeters (2025). County of Los Angeles Enterprise GIS. (2025, January 21). https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about



