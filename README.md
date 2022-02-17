# Homework_3
### Purpose

### Purpose

While static maps are useful for overserving conditions at a single point in time (or an average of a time span), it can sometimes be helpful to visualize changes in geospatial data from year to year. This notebook is intended to provide you with multiple examples of how to animate a time series. This lab will also show you one method to plot two separate datasets on the same graph to compare data.

For this exercise, we'll be subsetting and visualizing sea surface temperatures (SST) from the NOAA Optimum Interpolation 1/4 Degree Daily Sea Surface Temperature (OISST) Analysis, Version 2) and sea ice concentrations (SIC) data from the Monthly Mean Hadley Centre Sea Ice and SST dataset version 1 (HadISST1) data set. While this notebook will show you how to subset and visualize these datasets, ultimately, we hope that you can use this code as a reference guide to visualize any geospatial time-series dataset.

At the end of the lab, we will ideally have:

-	A GIF showing changes of sea surface temperatures over a 40-year timeframe;
-	A GIF showing of changes of sea ice concentrations over a 40-year timeframe; and
-	A graph showing the trend in sea surface temperatures and sea ice concentrations over time.

### Use Case Examples 

#### Geospatial GIFs 
GIFs are an effective tool in conveying a high density of information in a short amount of time. In the context of geospatial data, animated maps are often more effective at visualizing rates of change of information compared to static maps. For example, a GIF showing the movement of a hurricane towards the Eastern Seaboard would likely instill a greater sense of urgency in the public to be better prepared when the storm hits landfall than a static image of a tropical cyclone. In addition, GIFs often require little to no preamble to understand what is being visualized. This ease of understanding increases inclusivity and can minimize room for misinterpretation. Lastly, geospatial GIFs can also be used to help predict trends in spatial data. Having a way to quickly and effectively generate an animated spatial map can help contextualize data and give researchers a sense of what future data should look like.

#### Matplotlib Database Visualization
Multiple datasets can be plotted on the same Matplotlib plot, with different colors or shapes to distinguish between the datasets. This tool gives users a way to quickly and efficiently visualize and compare data with minimal data manipulation.

#### Sea Surface Temperature and Sea Ice Concentration Datasets 

As a standalone datasets, historical changes in sea surface temperature and sea ice concentrations can only tell you so much. But when these datasets are integrated and compared to each other and other global metrics, these datasets can offer insight into complex environmental models. For example, sea surface temperature and sea ice concentration can be utilized to help study:

- Likelihood of tropical cyclones formations (surface temperatures and humidity influence cyclones);
- Ocean acidification (warmer waters absorb more CO2);
- Volumetric changes in oceans (warmer waters expand volumetrically);
- Coral production rates (calcium carbonate formation is a function of temperature, acidity, depth (pressure));
- Reduction in sea ice volume and concentration;
- Inundation of coastal areas; and
- Changes in the transoceanic currents.

### Datasets

In this lab, we'll be using data from two sources.

•	SST: NOAA's 1/4° Daily Optimum Interpolation Sea Surface Temperature (OISST) version 2, or OISSTv2
•	SIC: Monthly Mean Hadley Centre Sea Ice and SST dataset version 1 (HadISST1)

Data Google Drive: https://drive.google.com/drive/folders/1bdVrH6EB0JAjreb0xAbcb6Nps5oyW2eW?usp=sharing

A description of each dataset is given below: 

### Sea Surface Temperature Data 

The NOAA 1/4° daily Optimum Interpolation Sea Surface Temperature (daily OISST) Climate Data Record (CDR) provides complete ocean temperature fields constructed by combining bias-adjusted observations from different platforms (satellites, ships, buoys) on a regular global grid, with gaps filled in by interpolation. The primary input source is satellite data from the Advanced Very High-Resolution Radiometer (AVHRR), which provides high temporal-spatial coverage from late 1981 to–present. This dataset is stored as NetCDF files (.nc files), including latitude and longitude coordinates, temperatures, and dates.

Metadata for the daily OISST is robust, with explanations of how data is acquired, the range of data, descriptions of how data was collected, contact information, and dataset constraints. 

Data source and metadata: NOAA National Centers for Environmental Information https://www.ncei.noaa.gov/metadata/geoportal/rest/metadata/item/gov.noaa.ncdc:C00844/html

NOAA Sea Surface Temperature Optimum Interpolation methods: https://www.ncei.noaa.gov/products/climate-data-records/sea-surface-temperature-optimum-interpolation


### Sea Ice Concentration Data

The Monthly Mean Hadley Centre Sea Ice and SST dataset version 1 (HadISST1) is one-half of the merged Hadley-OI sea surface temperature (SST) and sea ice concentration (SIC) dataset. The merged product provides monthly global mean sea surface temperature and sea ice concentration data from 1870 to the present. The merging procedure was designed to take full advantage of the higher-resolution SST information found in version 2 of the NOAA weekly optimum interpolation (OI) SST analysis, the other half of the merged dataset. The combined dataset blends historical SST and modern SST observations from ships, buoys, drifters, and sea ice observations, partly from the historical ship- and air-borne and partly from satellite data. This dataset is stored as NetCDF files (.nc files), including latitude and longitude coordinates, temperatures, and dates. Sea ice concentration is defined as ice located at the poles (approximately above and below 60 degrees latitude) regardless of continental or oceanic.

Metadata for the merged Hadley-OI sea surface temperature (SST) and sea ice concentration (SIC) dataset, in contrast to the daily OISST dataset, is slightly more challenging to understand without the familiarity of SST and SIC data collection techniques. Moreover, data collection techniques and constraints are not presented in the metadata; review papers of the dataset go into detail regarding these processes. The non-centralized metadata makes this dataset less accessible to the public. 

Data source and metadata: UCAR/NCAR - DASH Repository https://dashrepo.ucar.edu/dataset/158_asphilli.html

Journal of Climate article explaining why the datasets were merged: https://journals.ametsoc.org/view/journals/clim/21/19/2008jcli2292.1.xml


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/EDS220-Fall2021-org/Homework_3.git/HEAD)
