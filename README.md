# python-api-challenge

There are 2 parts to this challenge as listed below. Before going into either of those, please copy your weather_api_key and g_key in the respective folders (WeatherPy and VacationPy.

Part 1: WeatherPy

In this section, the Python script WeatherPy.ipynb will visualize the weather of 500+ cities of varying distance from the equator. To do so, I used a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and your problem-solving skills to create a representative model of weather across cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After each plot, amy obdersations and analysis was documented.

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, the linear regression is modelled. For example, described the relationships that I noticed and related findings.

Your final notebook must:

* Randomly select **at least** 500 unique (non-repeated) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed, with the city number and city name.
* Save a CSV(cities.csv) of all retrieved data and a PNG image for each scatter plot in the folder /output_data

Part 2:

Created a heat map that displays the humidity for every city from Part 1;

* Narrow down the DataFrame to find your ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

* Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**;
