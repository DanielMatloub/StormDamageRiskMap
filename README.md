# Storm Damage Risk Map
- Accesses forecast data of multiple National Oceanic and Atmospheric Administration (NOAA) websites, using the python requests module.
- Gets the data from the HTML code of the pages. 
- Filters the data to select the counties mentioned in the data.
- Finds coordinates of each county by reading a JSON file with that data.
- Determines how much impact the weather in each county will add to their risk of a blackout.
- Using all information gathered, uses the Python Folium library to build and return a heatmap map of all the data.

