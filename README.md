# Project background
Data's true power lies in its ability to definitively answer questions. This project leverages knowledge of Python requests, APIs, and JSON traversals to explore the fundamental question: "What is the weather like as we approach the equator?"

While it may seem obvious that temperatures increase near the equator, this project aims to provide concrete data and analysis to substantiate that claim.

## Instructions

This activity is broken down into two deliverables, WeatherPy and VacationPy.

**Part 1: WeatherPy**

In this deliverable, create a Python script to visualize the weather of over 500 cities of varying distances from the equator. Use the [citipy Python library](https://pypi.org/project/citipy/), the [OpenWeatherMap API](https://openweathermap.org/api), and your problem-solving skills to create a representative model of weather across cities.

**Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude**

Use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, create a series of scatter plots to showcase the following relationships:
* Latitude vs. Temperature
* Latitude vs. Humidity
* Latitude vs. Cloudiness
* Latitude vs. Wind Speed

**Requirement 2: Compute Linear Regression for Each Relationship**

To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.
Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r^2 values as you can see in the following image

[image](https://static.bc-edx.com/data/dl-1-2/m6/lms/img/linear-regression-plot.png)


Create the following plots:
* Northern Hemisphere: Temperature vs. Latitude
* Southern Hemisphere: Temperature vs. Latitude
* Northern Hemisphere: Humidity vs. Latitude
* Southern Hemisphere: Humidity vs. Latitude
* Northern Hemisphere: Cloudiness vs. Latitude
* Southern Hemisphere: Cloudiness vs. Latitude
* Northern Hemisphere: Wind Speed vs. Latitude
* Southern Hemisphere: Wind Speed vs. Latitude
After each pair of plots, explain what the linear regression is modeling. Describe relationships and other findings that was uncovered.

## Part 2: VacationPy

Complete the following steps:

1. Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

[Humidity map](https://static.bc-edx.com/data/dl-1-2/m6/lms/img/humidity_map.png)

2. Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
   - A max temperature lower than 27 degrees but higher than 21
   - Wind speed less than 4.5 m/s
   - Zero cloudiness

3. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
4. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
5. Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

[Hotel map](https://static.bc-edx.com/data/dl-1-2/m6/lms/img/hotel_map.png)

