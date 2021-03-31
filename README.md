# Citi_Bike_Station_Analysis_with_Tableau
Citi Bike Station Analysis with Tableau

## Table of Contents 
* [General Info](#General-info)  
* [Technologies](#technologies)  
* [Setup](#setup)  
* [Data Sources](#data-sources)
* [Overview](#overview)  

## General Info
This project is to make visualizations for the data from the NY Citi Bike website. The code used Pandas to format the data, and Tableau for all the visualization.  HTML with CSS and Bootstrap was used to make the web page. Data from June and July of 2018, 2019, and 2020 were used. Due to using the Public version of Tableau, there was a limit on how much data could be uploaded. June and July were selected as they are warmer months of the year, and there would likely be more activity to analyze. Three years were selected as 2020 is kind of an odd year due to the Covid-19 Coronavirus pandemic. There was interest in seeing how the 2020 data compared to 2019. 2018 was also used to make a better baseline for data when things are "normal." It was of great interest to see how the data might have changed with the pandemic during 2020. 

## Technologies
Project is created with:  
* Tableau Public 2021.1.0
* HTML5
* Bootstrap 5.0.0
* Pandas 
* Juptyer Notebook 6.0.3

## Setup
To view the project please follow either link: 
via Tableau Public: https://public.tableau.com/profile/alicia.perez2496#!/vizhome/Citi_Bike_Station_Analysis/Story1
via Github Pages: https://aliciaaperez.github.io/Citi_Bike_Station_Analysis_with_Tableau/


## Data Sources 
https://www.citibikenyc.com/system-data

## Overview
The data gathered was for June and July of 2018, 2019, and 2020. The data was downloaded from the listed website above, and modified in Jupyter Notebook with Pandas. That data was then loaded into Tableau Public to make visualizations. 

On the first slide of the story, we see the average trip duration for all the trips on a map using the start station and the end station. The map on the left is for the start stations, and the map on the right is for the end stations. The color varies based on the count of bike trips per station, and the size varies based on trip duration (in seconds). However, there were a few issues with the data. In the first section of the story, we can see that that a lot of the dots on the map are hard to see. This is because there is a good chunk of outlier data in which the average trip duration is skewed high due to someone having a bike much longer than normal. This might be due to people improperly locking or checking bikes in. It could also be due to bike theft. This brings us to the next page. In addition to the outliers in trip duration, there is one spot in Canada that a bike shows up at. The bikes were not meant to go that far, but a bicycle ended up in Canada. You can see it on both maps on the second part of the story labeled outliers. The one for the start stations is also impossible to see, but it is there. 
To combat the outliers, the maps were focused on the local bikes. Also, the trip duration data was filtered to remove anything over 7200 seconds or two hours. The data becomes much more clear on the map now. The time was chosen as per the website for this data (https://www.citibikenyc.com/how-it-works), the bicycles are meant to be used at a maximum of 30-45 minute rides. The cyclist can use them for longer at an additional cost. Two hours was chosen as a generous means to include anyone who rode the bike for longer. The data was tested with 3600 seconds, and there wasn't a huge difference, so for the sake of keeping more data 7200 seconds was used. 

The fourth part of the story shows the breakdown over the month and years for total rides. We can see that there was an increase in usage from 2018 to 2019. However, there was a drop in usage in 2020. Due to the pandemic, more people were staying home which correlates with bike usage.

The fifth panel of the story shows the gender breakdown of every trip. This data is by ride count. This is the gender per individual ride. There are duplicate riders. We can see that males are the most active users of the service. 

The sixth panel of the story is for the age breakdown. The age breakdown stays fairly consistent throughout the three years of data. The age used was the current age for today and not the age when the ride was taken. There is an interesting spike on the age of 51. It appears that there are a lot of people that age using the service. It could be one person using the service extremely consistent throughout the day. More investigation would be needed to see why there is such an anomaly in the data. 

The seventh panel of the story is for the age and gender breakdown. This further highlights that a person at age of 51 did not give a gender. 

There is a lot of data to be found with this dataset and many ways to look at the data depending on what kind of information you are looking for. Many more visualizations can be made to discuss the trajectory of this business. With the pandemic, bike usage took a hit, but there were still a lot of people using the service. Data for 2021 and 2022 would be of great interest to see how the data plots out over the next few years. Will the bike usage return to 2019 levels or increase from there? Or will bike usage continue to decrease? 