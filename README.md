
# 🌦️ Weather Data Extraction Tool  

*A Python script to fetch real-time weather data for any city or your current location using public APIs.*  

---

## 📌 Features  
- **City-based weather lookup**: Enter a city name to get temperature, humidity, wind speed, and conditions.  
- **Auto-location detection**: Fetches weather for your current location using IP geolocation.  
- **Multi-day forecast**: Shows a 3-day forecast with detailed time segments (morning/noon/evening/night).  
- **Clean output**: Displays data in both structured text and JSON formats.  

---

## 🛠️ Technologies Used  
- **Python 3**  
- `requests` library (HTTP API calls)  
- [wttr.in API](https://wttr.in) (Weather data)  
- [ipinfo.io API](https://ipinfo.io) (Geolocation)  

---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/weather-data-extractor.git  
   cd weather-data-extractor  
Install dependencies:


pip install requests  
Execute the script:


python weather_extractor.py  
📋 Example Usage
1. Fetch Weather for a Specific City
python
Enter City: london  
Temperature: 18 °C  
Weather: Cloudy  
Wind: 12 km/h  
Humidity: 65 %  
2. Auto-Detect Your Location's Weather
plaintext
Current Location: Tokyo  
Weather report: Tokyo  

                Light Rain  
       .-.      +22(21) °C  
    ― (   ) ―   ↗ 8 km/h  
       `-’     10 km  
      /   \    0.2 mm  
🧩 Code Snippets
Fetching Weather Data
python
import requests  
city = input("Enter City: ")  
response = requests.get(f"https://wttr.in/{city}?format=j1")  
data = response.json()  
print("Temperature:", data['current_condition'][0]['temp_C'], "°C")  
Auto-Detecting Location
python
res = requests.get('https://ipinfo.io/')  
city = res.json()['city']  
print("Current Location:", city)  
📂 Project Structure

weather-data-extractor/  
├── weather_extractor.py  # Main script  
├── README.md             # Documentation  
└── requirements.txt      # Dependencies  
🤝 Contribute
Fork the repo, add features (e.g., GUI, SMS alerts), and submit a PR!

Report bugs/issues here.

✨ Built with Python for API and data enthusiasts.


### Key Notes:  
1. Replace `your-username` with your GitHub username.  
2. For a **requirements.txt** file, add:  
   ```plaintext  
   requests==2.31.0  
