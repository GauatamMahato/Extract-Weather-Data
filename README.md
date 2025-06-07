Weather Data Extraction Tool
A Python-based application that fetches real-time weather data for any city or the user's current location using public APIs. The tool retrieves key weather metrics (temperature, humidity, wind speed, and conditions) and displays them in a structured format.

Features
City-Specific Weather: Enter a city name to get its current weather details.

Auto-Detection: Automatically fetches weather for the user's location using IP geolocation.

Multi-Day Forecast: Displays a detailed 3-day forecast with temperature ranges, wind speed, and conditions.

User-Friendly Output: Presents data in a clean, readable format (text-based or JSON).

Technologies Used
Python (Requests library for API calls)

wttr.in API (Weather data)

ipinfo.io API (Geolocation)

JSON Parsing (Handling API responses)

How It Works
The user inputs a city name or allows the script to detect their location.

The tool queries wttr.in for weather data and ipinfo.io for geolocation (if needed).

The response is parsed and displayed as:

Current weather (temperature, humidity, wind, conditions).

3-day forecast with time-specific details.

Installation & Usage
git clone https://github.com/your-username/weather-data-extractor.git  
cd weather-data-extractor  
pip install requests  
python weather_extractor.py  

Example Output
Enter City: delhi  
Temperature: 39 °C  
Weather: Haze  
Wind: 5 km/h  
Humidity: 28 %  

Use Cases
Personal weather checks via CLI.

Integration into larger apps (e.g., travel planners, event schedulers).

Learning API interaction and JSON handling in Python.

Why This Project?
Demonstrates API integration and data parsing skills.

Shows ability to build user-interactive CLI tools.

Easy to extend (e.g., add GUI, SMS alerts, or historical data analysis).

🔗 Try it out! Contribute or fork to enhance functionality.
