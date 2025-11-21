# Landsat True- and False-Color Imagery with Fire Perimeters in Los Angeles County
## About:
This repository houses code and materials for analyzing Landsat imagery, producing true-color and false-color composites, and mapping fire perimeters for the Eaton and Palisades fire boundaries:
- Working with NetCDF (.nc) Landsat data
- Reading and reprojecting shapefiles
- Creating RGB and false-color composites
- Overlaying geospatial data
- Generating publication-quality figures
- Writing clear and reproducible geospatial workflows

<img width="1200" height="630" alt="image" src="https://github.com/user-attachments/assets/ef4526e9-3516-44e5-881a-13693b844133" />


## Reprository Structure:
- When downloading data, add the data folder to `.gitignore` to reduce pushing big files onto github.

<img width="293" height="113" alt="Screenshot 2025-11-20 at 1 34 38 PM" src="https://github.com/user-attachments/assets/a9a13407-a309-4c96-8083-20143d6c9e56" />

# Packages Used:
In this notebook the packages were os, numpy, matplotlib.pyplot, geopandas, xarray, and rioxarray. If you are working on a server that already has `xarray` and `rioxarray`. Being able to import them onto the notebook book should be no issue. If you are working on a localized software for example `VS Code` and have not used `xarray` and `rioxarray` before. Follow these steps, on the terminal:

- Activate the EDS 220 conda environment and verify it is active.
- Install the netCDF4 package in the EDS 220 environment by running: `conda install -c conda-forge netcdf4`
- Verify that the netcdf4 package was installed.

#### References:
- Microsoft Planetary Computer. Planetary Computer. (n.d.). https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2 
- NPR. Satellite image ©2025 Maxar Technologies (January 9, 2025). https://www.kpbs.org/news/national/2025/01/09/photos-see-the-california-wildfires-destructive-force-in-satellite-images. 
- Palisades and eaton dissolved fire perimeters (2025). County Of Los Angeles Enterprise GIS. (2025, January 21). https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about 
