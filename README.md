# Storm Damage Risk Map
This Python script utilizes various weather advisory URLs from the National Weather Service (NWS) and county boundary data to generate a map using the folium library, showcasing areas affected by different weather advisories. The code extracts county-level information from the NWS advisories and maps the affected regions using polygons on a Folium map.

Dependencies:
requests
re
folium
geopy

Data Retrieval:
Scrapes specific NWS advisory URLs to extract affected areas' textual information.
Loads US county boundary data from a JSON file (us-county-boundaries.json).

Mapping Functionality:
Generates a Folium map and overlays polygons denoting affected counties based on different weather advisories.
Adjusts polygon weights and opacities to indicate varying advisory severity.

Instructions for Use:
Ensure the necessary libraries (requests, re, folium, geopy) are installed.
Make sure the us-county-boundaries.json file is present in the script's directory.
Run the script in a Python environment.
The script retrieves weather advisory information, maps the affected county areas, and generates an interactive Folium map displaying different advisories.

Code Structure Overview:
Weather Advisory URLs: NWS URLs for various weather advisories.
translateWeatherPage Function: Extracts affected areas from the NWS advisory pages.
findCounties Function: Matches extracted areas with county boundary data and returns relevant county names.
mapOutWeather Function: Maps the affected county areas onto a Folium map based on advisory severity.

Additional Notes:
Modify or expand the URLs for additional weather advisory types if required.
Adjust the weights and opacities within the mapOutWeather function to suit visual preferences or convey different advisory severity levels.
Ensure internet connectivity to retrieve live data from NWS advisory pages.
The generated map provides a visual representation of areas under different weather advisories, aiding in understanding the geographical scope and severity of weather alerts.

Note: The accuracy and completeness of the weather advisory data depend on the NWS advisory information and the provided county boundary dataset.








