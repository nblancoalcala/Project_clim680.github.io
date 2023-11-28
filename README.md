# The Relationship between Surface Temperature, Precipitation, and ENSO

### Noah Blanco-Alcalá
#### CLIM 680

## Introduction

This goal of this project is to look at the relationship between temperature and precipitation over land to determine if there has been an increase in either, and to determine if there is any correlation between them at a global scale. To do this, I will be looking at the trends overall (from 1979-2000), and it the perspective of two time periods. The first time period is from 1979-2000 and the second time period is from 2000-2014, and this is done to determine if there has been a bigger increase closer to the present. I will also be comparing these dataset sets to see if there is any significant differences during ENSO using the Niño 3.4 dataset.

## Data

The datasets I used are:

_Terrestrial Air Temperature and Precipitation_
The [University of Delaware's](https://www.psl.noaa.gov/data/gridded/data.UDel_AirT_Precip.html) Terrestrial Air Temperature and Precipitation dataset is monthly temperature and precipitation (only the temperature is used in this project) ranging from January 1900 to December 2014. It has a resolution of 0.5 degree latitude x 0.5 degree longitude global grid (720x360).

_GPCP Precipitation_
The Global Precipitation Climatology Project, or [GCPC](https://psl.noaa.gov/data/gridded/data.gpcp.html), is a monthly global precipitation dataset ranging from January 1979 to September 2023. It has a resolution of 2.5 degree latitude x 2.5 degree longitude global grid (144x72).

_Niño 3.4_
The Niño 3.4 is a climate index which represents the average equatorial SST's in the Pacific Ocean and is the most commonly used to define El Niño and La Niña events. This was found in the following path: '/home/lortizur/clim680/nino34_1982-2019.oisstv2_anoms.nc'

## Codes & Results

The code for this project can be found in this [notebook](https://github.com/nblancoalcala/Project_clim680.github.io/blob/master/project_clim680.ipynb)

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

## Code & Analysis

### Annual Air Temperature Mean
Overall: I calculated the overall mean air temperatures from 1900-2014 in °C. Here it is evident that the highest mean temperatures occur at the tropics, right next to the equator, while the lowest temperatures occur at the poles, especially Antarctica. With this I plotted a map of the monthly mean temperatures in the entire world, along with a time series plot of the overall global monthly mean air temperature.

1979-2000: I sliced the overall data into this first time period (TP1), from January 1979 to December 2000. I plotted a map and a time series plot of this data.

2000-2014: I sliced the overall data into this second time period (TP2), from January 2000 to December 2014. I plotted a map and a time series plot of this data.

Difference & Analysis: After plotting the data for both time periods, I then took the difference of the first time period from the second (TP2-TP1), and plotted the result into a map. Here we see that the temperatures of TP2 overall are slightly higher than the overall temperatures for TP1. The difference in temperature is as high as 7.3°C, likely in western Greenland or Northern Continental Russia, and as low as -6.16°C, likely in north eastern Antarctica, or north central continental Africa. The mean temperature difference is around 0.387°C, which can conclude that globally, there has been an average increase in air temperature by around 0.387°C from TP1 to TP2.


<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/d88ca57d-353f-4601-82b8-061487380d43">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/b6524870-f9dd-4a1b-915c-9e9c827ac277">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/5962c232-ce6d-4ab3-81b4-0b33ca63857c">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/1c994e6e-7252-487e-87b1-1ce6309cfa81">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/4998839f-1d5a-4e7a-819c-1a38829eec5a">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/efa96a6e-d66b-4704-922f-4e447b4575f0">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/06711f3a-fbf1-4734-9fed-fc72a8b45063">


### Annual Precipitation Mean

Method & Overall: I calculated the overall mean precipitation from 1979-2020 in millimeters per day (mm/day). Here it is evident that the highest mean precipitation occur near the equator in the Pacific, while the lowest mean precipitation occurs at the poles. With this I plotted a map of the monthly mean precipitation in the entire world, along with a time series plot of the overall global monthly mean precipitation.

1979-2000: I sliced the overall data into this first time period (TP1), from January 1979 to December 2000. I plotted a map and a time series plot of this data.

2000-2014: I sliced the overall data into this second time period (TP2), from January 2000 to December 2014. I plotted a map and a time series plot of this data.

Differences & Analysis: After plotting the data for both time periods, I again  took the difference of the first time period from the second (TP2-TP1), and plotted the result into a map. Here we can see that the biggest positive differences occur in the western Pacific, north of Australia and in the Oceania region, and the maximum value in the world is 1.49 mm/day. The biggest negative differences occur in the Southern Hemispheric equator, with the lowest value in the world being -1.76 mm/day. The mean precipitation difference is around 0.013 mm/day, and from this we can conclude that overall, globally there has be an increase in monthly mean precipitation by 0.013 mm/day, which is very negligible.

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/7b8b086a-9807-449f-9fc0-f18a5811f601">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/0657315d-e2d2-483e-8455-32a1bddf5994">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/e283c415-2cad-4e86-964d-552e0bde6405">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/8082976e-41d5-4ebb-be38-fe0255ea3a31">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/eb7ae79b-2b0e-4dc3-b25e-7840d3ca5eb3">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/08160e49-5283-4611-a69f-cb3a87de69f1">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/f202ce8b-604f-4f54-9d66-203eccf18216">

### Precipitation Anomalies & Climatology

Method: Precipitation climatology was calculated using the 'groupby' function, in which the time was grouped into months and the average was then taken by month. Precipitation Anomalies was calculated by grouping the precipitation data together by month, and subtracting that by the climatology.

Anomalies Analysis: I plotted a global map of precipitation anomalies from 1979-2020. It is shown here that the biggest precipitation anomalies occur in northern Australia, Oceania, and western Brazil, and the highest value is 37.7296 mm/day. The lowest anomalies occur in the central Indian Ocean, in a relatively similar region as the highest, with the lowest value being -18.9243 mm/day. The mean precipitation anomaly is around 2.6e-09, so it can be concluded that most over the world does not see a substantial change in precipitation throughout time.

Climatology Analysis: I plotted a 12-panel plot of monthly mean precipitation climatology, each panel being an individual month. The change in precipitation throughout the month stays very uniform in the equator, and there is not much change in the mid-latitudes either. The biggest differences can be seen near the Indian Ocean during the summer, and this can be attributed to the Indian Monsoon.

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/598f6baf-4f42-499d-bf52-96e3bcefe597">

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/4928dcb4-9c86-4b28-9cd5-ad05e065dcae">

### Correlation between Precipitation and Air Temperature

Method: A correlation was created here between temperature and precipitation by matching the time periods between both datasets, calculating climatology and anomolies (done before), creating a correlation variable through xarray, and plotting the correlation map of the entire world with significance (p-value of 0.05). In the map, the longitude is centered at 180°, because it appeared the smoothest at that location.

Analysis: Overall there is a very slight global correlation between precipitation and temperature. Some areas of extremes include Asia for the greatest positive correlation, and eastern Europe and the western coast of Europe for the greatest negative correlation. From this we can conclude that although in some areas temperature and precipitation may be correlated, overall most of the world does not have a strong correlation.

### Composite Precipitation Anomalies during ENSO

Method: To make a composite precipitation anomaly plot during ENSO, the precipitation data was sliced to match the time frame of the Niño 3.4 data. The the conditions of El Niño, La Niña, and neutral conditions were defined. Then, a composite was calculated for El Niño precipitation, La Niña precipiation, and neutral condition precipitation. The 3-panel plot was then created to view to the composite precipitation anomalies during ENSO.

Analysis: During El Niño, there is a clear increase in precipitation anomalies in the equatorial Pacific Ocean. During La Niña there is a slight decrease in precipitation in the equatorial Pacific Ocean, and not much change anywhere else. In neutral conditions there is not much difference in precipitation anomalies, which makes sense considering that neutral conditions will likely bring average amounts of rainfall, and that there are many more instances of neutral conditions than El Niño or La Niña.

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/daf08a13-57a9-4b77-8e2d-4a7e01b917b7">


### Composite Temperature Anomalies during ENSO

Method: To make a composite temperature anomaly plot during ENSO, the temperature data was sliced to match the time frame of the Niño 3.4 data. The the conditions of El Niño, La Niña, and neutral conditions were defined. Then, a composite was calculated for El Niño temperature, La Niña temperature, and neutral condition temperature. The 3-panel plot was then created to view to the composite temperature anomalies during ENSO. To note, only the land surface data is observed.

Analysis: During El Niño, there is are large positive temperature anomalies in the continental United States, and there are slight negative temperature anomalies in eastern Russia and Antarctica. During La Niña, the temperature anomalies are not as extreme, but the highest positive anomalies occur in eastern Russia, and highest negative anomalies occur in Antarctica. During neutral conditions, theres are extreme temperature anomalies in central Russia and Alaska, with highest negative anomalies occuring in Antarctica.

<img width="314" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/aec5a047-4f0d-453b-b00f-dbb0e53d6e93">

### Composite Temperature Differences between El Niño and Neutral, & La Niña and Neutral

Method: From the previously created composites between ENSO and temperature anomalies, I calculated the difference by created a variable and making it equal to the Neutral composite minus the El Niño composite, and again with Neutral composite minus La Niña composite. I plotted both composites on a 2 panel plot, and I plotted the composites with significance using a p-value of 0.05.

Analysis: For the difference between neutral and El Niño, there are very large negative difference in the United States, and large postive differences in Northern Europe. With this we can confirm that the temperatures during El Niño in the U.S. are higher than in neutral conditions, and in Europe, the temperatures and lower. For the difference between neutral and La Niña, there are large positive difference in northern Europe (close to/in Russia), and in Alaska/NW Canada. Here we can conclude that during La Niña, the temperatures of these places are colder than in neutral conditions.

<img width="314" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/b7efdd86-2335-4628-9919-6783e9ff2e5f">

<img width="429" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/eaca9595-e285-46a0-994e-5a1c2e7198ef">

<img width="429" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/b988f2c1-3229-456a-803e-72c7ec91b9b8">

### Correlation between Niño 3.4 and Temperature Anomalies

Method: I created a correlation between the Niño 3.4 and temperature anomalies using Xarray and plotted the global correlation.

Analysis: In northern South America there is a very strong correlation between ENSO and temperature anomalies. In other parts of the world the positive and negative correlations are not as strong. We can gather that in most regions in the world there is not a big correlation between land air temperature and ENSO, but in some regions there are hotspots where they are correlated.

<img width="468" alt="image" src="https://github.com/nblancoalcala/Project_clim680.github.io/assets/142943512/9e5f9e57-8afd-49ee-b4e4-1a87e3c7b992">

## Conclusion & Summary
Summary:
Using the data and plots from this project, we can conclude that air temperatures over land surfaces have increased over time, but that precipitation is not as correlated with temperature as I initially expected. There are other factors that go into the change in precipitation with time, which could be investigated further in future studies. With the ENSO data, the results were more expected in that El Niño brings more rain to the Pacific, while La Niña brings less. It also confirmed known temperatures trends as well, in that in an El Niño the continental United States typically sees warmer winters. 

In future projects and analysis regarding this topic, an improvement could have been to include composites between Niño 3.4 and Precipitation anomalies, which couldn't be completed in this project due to time constraints. 

Issues: 
The biggest issue I encountered was calculating and plotting the significance, I have a lot of trouble getting it to work with the data that I had. The creation of the Github page/report was also very challenging initially, but once I got it to work, I was able to fill it in and complete it very quickly.

