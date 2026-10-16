
# SkyCast: Weather App

A weather app built with HTML, CSS and JavaScript. Search for any city to see the current weather and a 5-day forecast.

**Live demo:** https://samiuallahganaie.github.io/weather-app/

## Features
- Current temperature, "feels like", humidity, wind speed and conditions
- 5-day forecast with high and low temperatures
- Switch between Celsius and Fahrenheit (your choice is remembered)
- "Use my location" button that uses the browser's location feature
- Other matching cities shown when a name is shared by more than one place
- Last 5 searches saved in the browser
- Background colour changes with the weather and the time of day
- Clear error messages for unknown cities and connection problems
- Responsive layout for phones and desktops

## How it works
The app calls two free [Open-Meteo](https://open-meteo.com/) APIs with `fetch`:
1. the Geocoding API turns a city name into coordinates
2. the Forecast API returns the current weather and the daily forecast for those coordinates

No account or API key is needed.

## Run it locally
No installation is needed. Download the repository and open `index.html` in a browser. An internet connection is required to load the weather data.

## What I practised
- Calling web APIs with `fetch`, `async` / `await` and `AbortController` timeouts
- Handling loading states, empty results and network errors
- Saving settings and recent searches with `localStorage`
- Building the page safely with `textContent` instead of inserting raw HTML
- Using the Geolocation API
- Responsive design with CSS Grid and Flexbox

## Credits
Weather data by [Open-Meteo.com](https://open-meteo.com/).

