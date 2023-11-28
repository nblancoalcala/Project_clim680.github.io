# The Relationship between Surface Temperature, Precipitation, and ENSO

### Noah Blanco-Alcalá
#### CLIM 680

## Introduction

This goal of this project is to look at the relationship between temperature and precipitation over land to determine if there has been an increase in either, and to determine if there is any correlation between them at a global scale. To do this, I will be looking at the trends overall (from 1979-2000), and it the perspective of two time periods. The first time period is from 1979-2000 and the second time period is from 2000-2014, and this is done to determine if there has been a bigger increase closer to the present. I will also be comparing these dataset sets to see if there is any significant differences during ENSO using the Niño 3.4 dataset.

## Data

The datasets I used are:

_Terrestrial Air Temperature and Precipitation_
The [University of Delaware's] (https://www.psl.noaa.gov/data/gridded/data.UDel_AirT_Precip.html) Terrestrial Air Temperature and Precipitation dataset is monthly temperature and precipitation (only the temperature is used in this project) ranging from January 1900 to December 2014. It has a resolution of 0.5 degree latitude x 0.5 degree longitude global grid (720x360).

_GPCP Precipitation_
The Global Precipitation Climatology Project, or [GCPC] (https://psl.noaa.gov/data/gridded/data.gpcp.html), is a monthly global precipitation dataset ranging from January 1979 to September 2023. It has a resolution of 2.5 degree latitude x 2.5 degree longitude global grid (144x72).




## Results & Codes

#### Functions
A few of the functions that were created in this project include:
* Labeling plots
* Adding lines of latitude and longitude
* Creating climatologies and anomalies
* Slicing datasets into previously defined time periods

#### Conda Environment 
The environment.yml file lists all of modules needed to run the code. This includes:
* Xarray
* Numpy
* Scipy
* Matplotlib
* Etc. (refer to environment.yml)

## Analysis

### Annual Precipitation Mean

### Annual Air Temperature Mean

### Air Temperature Climatology

### Precipitation Climatology

### Correlation between Precipitation and Air Temperature

### Composite Precipitation Anomalies during ENSO

### Composite Temperature Anomalies during ENSO

### Composite Temperature Differences between El Niño and Neutral

### Composite Temperature Differences between La Niña and Neutral

### Correlation between Niño 3.4 and Temperature Anomalies
