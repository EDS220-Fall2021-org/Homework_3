# Homework_3
### Purpose

While static maps are useful for oberserving conditons at a single point in time (or an average of a time span), it can sometimes be helpful to visualize changes in geospatial data from year to year. This notebook is intended to provide you with multiple examples of how to animate a timeseries. This lab will also show you one method to plot two seperate datasets on the same graph to compare data.  

For this exercise, we'll be subsetting and visualsing sea surface temperatures (SST) from the NOAA Optimum Interpolation 1/4 Degree Daily Sea Surface Temperature (OISST) Analysis, Version 2) and sea ice concentrations (SIC) data from the Monthly Mean Hadley Centre Sea Ice and SST dataset version 1 (HadISST1) data set. 

At the end of the lab, we will ideally have: 

- A gif showing changes of sea surface temperatures over a 40-year timeframe; 


- A gif showing of changes of sea ice concentrations over a 40-year timeframe; and


- A graph showing the trend in sea surface temperatures and sea ice concentrations over time.

### Use Case Examples 

Gifs are an effective tool in conveying a high density of information in a short amount of time. In the context of geospatial data, animated maps are often more effective at visualizing rates of change of information compared to static maps. For example, a gif showing the movement of a hurricane towards the Eastern Seabord would likely instill a greater sense of urgency in the public to be better prepared when the storm hits landfall than a static image of a tropical cyclone. In addition, gifs often require little to no preamble to understand what is being visualized. This ease of understanding increases inclusivity and can minimize room for misinterpretation. Lastly, geospatial gifs can also be used to help predict trends in spatial data. Having a way to quickly and effectively generate an animated spatial map can help contextualize data and give researchers a sense of what future data should look like.

### Datasets

In this lab, we'll be using data from two sources. 
- SST: NOAA's 1/4° Daily Optimum Interpolation Sea Surface Temperature (OISST) version 2, or OISSTv2
- SIC: Monthly Mean Hadley Centre Sea Ice and SST dataset version 1 (HadISST1)

Data Google Drive: https://drive.google.com/drive/folders/1bdVrH6EB0JAjreb0xAbcb6Nps5oyW2eW?usp=sharing

A description of each dataset is given below: 

### Sea Surface Temperature Data 

The NOAA 1/4° daily Optimum Interpolation Sea Surface Temperature (daily OISST) Climate Data Record (CDR) provides complete ocean temperature fields constructed by combining bias-adjusted observations from different platforms (satellites, ships, buoys) on a regular global grid, with gaps filled in by interpolation. The main input source is satellite data from the Advanced Very High-Resolution Radiometer (AVHRR), which provides high temporal-spatial coverage from late 1981 to–present. 
This dataset is stored as NetCDF files (.nc files) that include latitude and longitude coordinates, temperatures, and dates.

Data source and metadata: NOAA National Centers for Environemntal Information https://www.ncei.noaa.gov/metadata/geoportal/rest/metadata/item/gov.noaa.ncdc:C00844/html

NOAA Sea Surface Temperature Optimum Interpolation methods: https://www.ncei.noaa.gov/products/climate-data-records/sea-surface-temperature-optimum-interpolation


### Sea Ice Concentration 

The Monthly Mean Hadley Centre Sea Ice and SST dataset version 1 (HadISST1) is one half of the merged Hadley-OI sea surface temperature (SST) and sea ice concentration (SIC) dataset. The merged product provides monthly global mean sea surface temperature and sea ice concentration data from 1870 to the present. The merging procedure was designed to take full advantage of the higher-resolution SST information found in version 2 of the NOAA weekly optimum interpolation (OI) SST analysis, the other half of the merged dataset. The combined dataset blends historical SST and modern SST observations from ships, buoys, drifters, and sea ice observations, partly from historical ship- and air-borne and partly from satellite data.This dataset is stored as NetCDF files (.nc files) that include latitude and longitude coordinates, temperatures, and dates.

Data source and metadata: UCAR/NCAR - DASH Repository
https://dashrepo.ucar.edu/dataset/158_asphilli.html

Journal of Climate article explaining why the datsets were merged: https://journals.ametsoc.org/view/journals/clim/21/19/2008jcli2292.1.xml

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/EDS220-Fall2021-org/Homework_3.git/HEAD)
