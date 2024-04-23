# python-api-challenge
 
The first part, WeatherPy, of this project obtains weather from "OpenWeatherMap API" and creating a new dataframe then putting that into a CSV file to be read in the second part of the project VacationPy. VacationPy locates hotels using Geoapify API to plan a hotel that fit specific conditions.

# WeatherPy

## Obtaining Data
Citipy generates random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

## Plotting Relationships
Used the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. 

Create a series of scatter plots to showcase the following relationships:
    Latitude vs. Temperature
    Latitude vs. Humidity
    Latitude vs. Cloudiness
    Latitude vs. Wind Speed

## Compute Linear Regression for Each Relationship
Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude)

Creat a series of plots showing the following
    Northern Hemisphere: Temperature vs. Latitude
    Southern Hemisphere: Temperature vs. Latitude
    Northern Hemisphere: Humidity vs. Latitude
    Southern Hemisphere: Humidity vs. Latitude
    Northern Hemisphere: Cloudiness vs. Latitude
    Southern Hemisphere: Cloudiness vs. Latitude
    Northern Hemisphere: Wind Speed vs. Latitude
    Southern Hemisphere: Wind Speed vs. Latitude

# Vacationpy
Using the CSV file from Part 1 and Geoapify API and geoViews Python library to map points to plan future vacations matching a certain criteria

## Mapping
Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
    A max temperature lower than 27 degrees but higher than 21
    Wind speed less than 4.5 m/s
    Zero cloudiness

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:    

