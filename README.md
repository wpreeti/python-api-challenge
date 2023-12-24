# python_api_challenge

Part I - WeatherPy

Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator.  Utilized OpenWeatherMap API, a Python library to create a representative model of weather across world cities.

Built a series of scatter plots to showcase the following relationships:
Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude
Ran linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):
Northern Hemisphere - Temperature vs. Latitude
Southern Hemisphere - Temperature vs. Latitude
Northern Hemisphere - Humidity vs. Latitude
Southern Hemisphere - Humidity vs. Latitude
Northern Hemisphere - Cloudiness vs. Latitude
Southern Hemisphere - Cloudiness vs. Latitude
Northern Hemisphere - Wind Speed vs. Latitude
Southern Hemisphere - Wind Speed vs. Latitude


Randomly selected 500+ unique (non-repeat) cities based on latitude and longitude.
Performed a weather check on each of the cities using a series of successive API calls. Created a print log of each city as it's being processed with the city number and city name. Saved a CSV of all retrieved data and a PNG image for each scatter plot.

Part II - VacationPy

Created a heat map that displays the humidity for every city generated from Part I - WeatherPy.

Narrowed down the DataFrame to find an ideal weather condition. For example:

A max temperature lower than 80 degrees but higher than 70.
Wind speed less than 10 mph.
Zero cloudiness.
Using Google Places API located the first hotel for each city located within 5000 meters of your coordinates.

Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.


Requirements:

Install citypy in python environment (https://pypi.python.org/pypi/citipy)
OpenWeatherMap API Key (https://openweathermap.org/) as 'weather_api_key'
Google API Key (https://console.developers.google.com/getting-started) as 'geoapify_key'
Create API Keys and store it in the 'api_keys.py' file before running the Jupyter notebooks.
