
# Weather App

A simple, responsive weather application that provides real-time weather information for any city, as well as weather updates based on the user's current location. The app displays various weather details such as temperature, humidity, UV index, wind speed, and sunset time, with an hourly forecast layout.

## Features

- **Search by City Name:** Users can input a city name to retrieve current weather data for that location.
- **Geolocation-based Weather:** Automatically fetches weather information based on the user's current geographic location.
- **24-Hour Forecast:** Displays temperature, wind speed, and weather icons for each hour of the day.
- **Weather Details:** Provides additional weather information such as UV index, humidity, real feel, wind speed, sunset time, and pressure.
- **Dynamic Weather Icons:** Updates the weather icons based on the current weather conditions (clear, cloudy, rainy, etc.).

## Screenshots

### Main UI
![Screenshot (100)](https://github.com/user-attachments/assets/14fd561a-9aa1-4d2f-b923-cd141ff3fcd1)

### Weather Details
![Details](![Screenshot (101)](https://github.com/user-attachments/assets/d1036c3c-64d9-428f-8358-3b870dc743f8)
)

## How to Use

1. **Clone the repository:**
   ```
   git clone https://github.com/yourusername/weather-app.git
   cd weather-app
   ```

2. **API Key Setup:**
   - Sign up for a free account at [OpenWeatherMap](https://openweathermap.org/) to obtain your API key.
   - Replace the placeholder `apiKey` in the script section of `weatherui2.html` with your actual API key:
     ```javascript
     const apiKey = 'your-api-key-here';
     ```

3. **Open the Application:**
   - Open `weatherui2.html` in your preferred web browser to view the app.
   - The app will initially attempt to use your geolocation to provide weather updates, with the option to search for other cities using the search bar.

## File Structure

```
weather-app/
├── index.html                # Entry point of the app
├── weatherui2.html           # Main weather interface
├── styles.css                # Stylesheet for the app
├── images/                   # Directory for icons and images
│   ├── search.png
│   ├── clear.png
│   ├── clouds.png
│   ├── rain.png
│   ├── default.png
├── README.md                 # Documentation
```

## HTML File Details

- **`index.html`:** 
  - Initial landing page of the app (you can customize it further to provide an overview or redirection to the main weather interface).
  
- **`weatherui2.html`:**
  - Main weather interface where the user can search for cities and view weather details. 
  - It uses OpenWeatherMap's API to fetch weather data and displays it dynamically.

## Scripts

- **Weather Data Fetching:**
  The weather data is fetched using the OpenWeatherMap API with the help of `fetchWeather()` and `getWeatherData()` functions.

- **Geolocation:**
  If geolocation access is allowed by the user, the app automatically fetches weather data for the user's current location.

- **Search Weather:**
  Users can search for weather data by entering a city name into the search bar and pressing Enter or clicking the search button.

## Technologies Used

- **HTML5** for structure.
- **CSS3** for styling and layout.
- **JavaScript** for dynamic content and API integration.
- **OpenWeatherMap API** for weather data.

## Future Enhancements

- **Extended Forecast:** Expand the app to display a 7-day forecast.
- **Improved Error Handling:** Provide more user-friendly messages when weather data cannot be fetched.
- **Real-Time Updates:** Implement real-time weather updates without requiring a page refresh.

