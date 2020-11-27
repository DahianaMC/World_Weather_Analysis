# World_Weather_Analysis
## Background
The requirement for this challenge is to add more data to the database, or cities DataFrame, so that customers know the weather in the cities when they click on a pop-up marker. Also I need to add the amount of rainfall or snowfall within the last three hours so that customers can filter the DataFrame using input statements based on the temperature range and whether or not it is raining or snowing. Finally, you’ll need to create a directions layer Google map that shows the directions between multiple cities for travel.

## Objectives
The goals are:

- Use nested try-except blocks.
- Use Pandas methods and attributes on a DataFrame or Series.
- Create a new DataFrame from a new API search with new weather parameters.
- Filter DataFrames based on input and nested decision statements, and logical expressions.
- Create pop-up markers on a Google map from a filtered DataFrame.
- Add a directions layer on a Google map between cities in the filtered DataFrame.

## Results
- Get the Weather Description and Amount of Precipitation for Each City.
  - Jupyter notebook: Weather_Database.ipynb
  - Generate a dataset of 1,500 random latitudes and longitudes.
  - Get the nearest city using the citipy module.
  - Perform an API call with the OpenWeatherMap.
  - Retrieve the following information from the API call:
    - Latitude and longitude
    - Maximum temperature
    - Percent humidity
    - Percent cloudiness
    - Wind speed
    - Weather description (e.g., clouds, fog, light rain, clear sky)
    - The amount of rainfall over the last hour (1 hr).
    - The amount of snowfall over the last hour (1 hr)
   - Export dataframe and save as WeatherPy_database.csv
 
 - Have Customers Narrow Their Travel Searches Based on Temperature and Precipitation.
  - Jupyter notebook: Vacation_Search.ipynb
  - Use the dataframe generated from Weather_Database.ipynb and import as new dataframe.
  - Filter the DataFrame for minimum and maximum temperature preferences, and if the rain or snow accumulation is 0 inches or not using conditional statements.
  - Add the cities to a marker layer map with a pop-up marker for each city that includes: Hotel name, City, Country, Current weather description with the maximum temperature.
  - New marker layer map was saved as WeatherPy_vacation_map.png
  - Export dataframe and save as WeatherPy_vacation.csv.
  
- Create a Travel Itinerary with a Corresponding Map.
  - Create a map (travel itinerary) that shows the route between four cities from the customer’s possible travel destinations, and then create a map with pop-up markers for the four cities.
  - Jupyter notebook: Vacation_Itinerary.ipynb.
  - Use the dataframe created from WeatherPy_vacation.csv.
  - Choose 4 cities, should be close together to get the direction map.
  - Create a marker layer map for the four cities.
  - Screenshot of the route it was saved as WeatherPy_travel_map_markers.png.
  - 
