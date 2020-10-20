# Weather and Vacation API
What is weather like as you approach the equator? In the below analysis I review weather factors in over 600 cities around the world at varying latitudes and longitudes to see how the temperature, humidity, cloudiness and wind speed are effected as you get closer and farther from the equator.  
  *Below data is a snapshot of data pulled on 10/17/20. Running notebook may result in different results.*

![Big Map](Images/equatorsign.png)

## Table of contents
* [About Weather](#about_weather)
* [Weather by Hemisphere](#weather_by_hemisphere)
* [Ideal Weather](#ideal_weather)
* [Vacation Spots](#vacataion_spots)
* [Conclusion](#conclusion)
* [Jupyter Notebooks](#jupyter_notebooks)
* [Sources](#sources)
* [Contact](#contact)


## About Weather
To gather my random world wide city data, I used a `.random.uniform` function to pull a set of 624 cities from varying latitudes and longitudes. Once I compiled this list, I ran a `for loop` to gather data on each city’s maximum temperature, humidity percent level, cloudiness percent, and wind speed. I added this information to a `DataFrame` to analyze. Due to limitations in pulling the data, I added `time.sleep()` after every 50 cities pulled in my code so that I would not exceed my limit of data pulls from the OpenWeatherMap API. 

![Cities](Images/cities_df.PNG)

I then used the `py.plt` function to show my data in scatter plots below. 

Within my data set of 624 random cities all over the world, there is a correlation between the city’s Latitude with the temperature. As the city becomes closer to the equator (latitude of 0) the temperature increases. As the city locations move farther away from the equator, the temperature decreases. My data set has more data for the Northern Hemisphere and the coldest max temperatures can be found at a latitude location of 80. 

![lat vs temp](Images/lat_temp.PNG)

Although humidity can be high at all Latitude locations, at the equator it is consistently high and there is no data to suggest low humidity near 0 latitude. 

![humidity](Images/lat_humidity.PNG)

There appears to be no real correlation to of Cloudiness to latitude accept that at the equator, like humidity, there appears to always be a percent of cloud formation.

![cloudiness](Images/lat_cloudiness.PNG

There is no correlation between wind speed and latitude. There are some outlying data points in the upper norther hemisphere. 

![wind speed](Images/lat_wind.PNG)

## Weather by Hemisphere

![north temp](Images/north_temp_r.PNG)
![south temp](Images/south_temp_r.PNG)

![north humidity](Images/north_humidity_r.PNG)
![south humidity](Images/south_humidity_r.PNG)

![north cloudiness](Images/north_cloudiness_r.PNG)
![south cloudiness](Images/south_cloudiness_r.PNG)

![north wind speed](Images/north_wind_r.PNG)
![south windspeed](Images/south_wind_r.png)

![heat map](Images/heat_map_snip.PNG)

## Ideal Weather
![ideal_temp](Images/ideal_temp.PNG)


## Vacation Spots

![hotels](Images/hotels.PNG)
![hotels map](Images/ideal_hotel.PNG)
![hotel box](Images/hotel_box.PNG)

## Conclusion

## Jupyter Notebooks

## Sources
 OpenWeatherMap API
 
 Google Places API
 
## Contact
Sara Simoes
