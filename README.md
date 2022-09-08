## API-Targeting Holiday Location


## Background
Whether, financial, political, or social data's true power rests in its ability to answer questions definitively. When people plan holidays,they do not want their vacations to be spoiled by bad weather. Here is the task for me to pick out suitable cities to travel while the weather conditions match my preference.


### Source

1.Randomly pick over 500 cities.
2.Make API calls from Openweather to get cities' weather conditions.


### Data Analysis

1.Latitude vs. Temperature Plot  
![ALT](https://github.com/LynHJ/API/blob/bf09f21c59a5918d28f70d477b96aa4da4af3d8a/WeatherPy/Output%20Data/LatMaxt.png)  
Note:  
The picture above shows two indications. One is that the maximum of cities' temperature is vary with their latitude.Another point is we can find most of the people's active regions are in the Northern hemisphere as there is no city in between 60 to 80 southern latitude while there are some cities still in between 60 to 80 northern latitude.  

2.Latitude vs. Humidity Plot  
![ALT](https://github.com/LynHJ/API/blob/bf09f21c59a5918d28f70d477b96aa4da4af3d8a/WeatherPy/Output%20Data/LatHumi.png)  
Note:  
The picture above shows two indications. One is that cities' humidity is not highly related with their latitude.Another point is that the humidity in the range between 20 to 50 northern latitude  and the range between 0 to 20 southern latitude are unstable. Based on the second point, we could find out that those ranges match with the distribution of globe land and help us to conclude that the ocean could stabilize the climate change.  

3.Latitude vs. Cloudiness Plot  
![ALT](https://github.com/LynHJ/API/blob/bf09f21c59a5918d28f70d477b96aa4da4af3d8a/WeatherPy/Output%20Data/LatCloud.png)  
Note:  
The picture above shows that cities' cloudness is not related with their latitude.  

4.Latitude vs. Wind Speed Plot  
![ALT](https://github.com/LynHJ/API/blob/bf09f21c59a5918d28f70d477b96aa4da4af3d8a/WeatherPy/Output%20Data/LatWindSd.png)  
Note:  
The picture above shows that cities' Wind Speed is not related with their latitude. The city data with 17.5(mph)wind speed might be a outlier. We need more detial of that city to make a clear conclusion.  

### Advanced Data Analysis

Setting up my prefered weather condition  
1. Temperature:21~27  
2. Wind Speed:<4.5  
3. Cloudiness: 0  

![ALT](https://github.com/LynHJ/API-Targeting-Holiday-Location/blob/0661cc4af97bbbf1dee09abbd93f650713a68221/WeatherPy/Image/Heatmap_layer.png)  

#### Summary

1. Using perference to target cities.  
2. Using Targeted cities to discover nearest hotel.  
3. Using gmap.marker_layer to store all the information. 

![ALT](https://github.com/LynHJ/API/blob/bf09f21c59a5918d28f70d477b96aa4da4af3d8a/WeatherPy/Image/Marker_Layer.png)

## Content:

Project  
|  
|-&nbsp;WeatherPy|  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-VacationPy.ipynb  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-WeatherPy.ipynb   
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-OutputData:|-CityData.csv  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-LatCloud.png  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-LatHumi.png    
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-LatMaxt.png  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-LatWindSd.png    
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-Image:&emsp;&emsp;&nbsp;|-Heatmap_layer.png  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-Marker_Layer.png  
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|-requirements.txt    
|-.gitignore  
|-README.md   

## Installation

pip install -r requirements.txt  

## Prerequisites

1. Get a free API Key at https://cloud.google.com/maps-platform/
&emsp;Clone the repo
&emsp;git clone https://github.com/your_username_/Project-Name.git
&emsp;Create a api-keys.py to put your API in
&emsp;gkey = 'ENTER YOUR API'
 
2. register Openweather API



