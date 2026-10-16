# SkyCast: Weather App

A weather app built with HTML, CSS and JavaScript. Search for any place, not only cities, to see the current weather and a 5-day forecast.

**Live demo:** https://samiuallahganaie.github.io/weather-app/

## Features
- Search any place: cities, towns, villages, areas, landmarks, postcodes, or exact coordinates such as `34.19, 74.36`
- Each result shows what kind of place it is (for example Village or Attraction)
- Current temperature, "feels like", humidity, wind speed and conditions
- 5-day forecast with high and low temperatures
- Switch between Celsius and Fahrenheit (your choice is remembered)
- "Use my location" button that uses the browser's location feature
- Other matching places shown when a name is shared by more than one place
- Last 5 searches saved in the browser
- Background colour changes with the weather and the time of day
- Clear error messages for unknown cities and connection problems
- Responsive layout for phones and desktops

## How it works
The app calls free web APIs with `fetch`:
1. [OpenStreetMap Nominatim](https://nominatim.org/) turns a place name or postcode into coordinates. This is what lets you search villages, landmarks and areas.
2. If that search finds nothing or is unavailable, the app falls back to the [Open-Meteo](https://open-meteo.com/) Geocoding API for city names.
3. The Open-Meteo Forecast API returns the current weather and the daily forecast for those coordinates.
4. If you type coordinates, the app skips the search and loads the weather directly.

No account or API key is needed.

## Run it locally
No installation is needed. Download the repository and open `index.html` in a browser. An internet connection is required to load the weather data.

## What I practised
- Calling web APIs with `fetch`, `async` / `await` and `AbortController` timeouts
- Combining two services with a fallback when one fails
- Handling loading states, empty results and network errors
- Saving settings and recent searches with `localStorage`
- Building the page safely with `textContent` instead of inserting raw HTML
- Using the Geolocation API
- Responsive design with CSS Grid and Flexbox

## Credits
Weather data by [Open-Meteo.com](https://open-meteo.com/). Place data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright).
