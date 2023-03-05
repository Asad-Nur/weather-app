Weather App
This is a simple Python script that uses the OpenWeatherMap API to retrieve and display the weather and temperature for a given city.

Requirements
Python 3.6 or later
requests module (install with pip install requests)
Usage
Obtain an API key from OpenWeatherMap by signing up for a free account on their website.
Replace API_KEY in the code with your API key.
Run the script: python weather.py
Enter a city name when prompted.
Output
The script will output the weather and temperature for the given city, or an error message if the city is not found or there is an issue with the API request.

Notes
The temperature is returned in Celsius.
The weather description is based on the current weather conditions (e.g., "clear sky", "few clouds", "rain").
