# python_api_challenge

This challenge included two parts, WeatherPy and VacationPy. 

## WeatherPy:
Utilizing the citipy Python library we generated a list of cities located within 90 degrees latitude of the equator. We then utilized the openweathermap.org API to retrieve weather information on the cities found using citipy. The complete dataset contained the weather for over 500 cities located near the equator which was saved to a DataFrame and exported to a csv file.

This data was then used to create and export a series of scatter plots comparing latitude to temperature, humidity, cloud cover, and wind speed.

The data was then separated into two new DataFrames, one for cities in the Northern Hemisphere and one for cities in the Southern Hemisphere. This allowed us to compute the linear relationship between weather and proximity to the equator. Scatter plots containing linear regression lines were generated for temperature, humidity, cloud cover, and wind speed versus latitude separately for the Northern and Southern Hemisphere. The strongest linear relationship was found between temperature and latitude in the Northern Hemisphere with temperatures increasing closer to the equator.

## VacationPy:
For this challenge we created several maps using Geoapify API and the geoViews Python library. We started by creating a world map displaying the humidity for a list of cities. We then created a DataFrame containing cities with “ideal” weather, between 21 and 27 degrees Celsius with no clouds and a wind speed less than 4.5 m/s.

Using this new data set we ran an API request from Geoapify to find the nearest hotel to each location and added the hotel name to our DataFrame. Finally we recreated the first world map with our new DataFrame of ideal weather conditions and added a hover message containing the hotel name.

