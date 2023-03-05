import requests
import json

# API key and base URL for the OpenWeatherMap API
API_KEY = "your_api_key_here"
BASE_URL = "http://api.openweathermap.org/data/2.5/weather"

# Get city name from the user
city = input("Enter a city name: ")

# Build the request URL using the API key and city name
request_url = f"{BASE_URL}?appid={API_KEY}&q={city}"

# Make a GET request to the API
response = requests.get(request_url)

# Print the status code of the response
print("Status code:", response.status_code)

# If the request was successful (status code 200), parse the response and print the weather and temperature
if response.status_code == 200:
    data = json.loads(response.text)
    weather = data['weather'][0]['description']
    temperature = round(data["main"]["temp"] - 273.15, 2)
    print("Weather:", weather)
    print("Temperature:", temperature, "celsius")

# If the request was not successful, print an error message
else:
    print("An error occurred.")
