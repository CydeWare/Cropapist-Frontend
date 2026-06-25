# Cropapist-Frontend

---

# Cropapist

Cropapist is a web-based crop yield prediction application powered by machine learning. Given a location and a crop type, it estimates the expected annual yield in hg/ha based on real-time weather data fetched for that location.

## Features

- **Interactive map** — click anywhere on the map to select a location, or enter coordinates manually
- **Crop selection** — choose from 10 supported crop types including Maize, Rice, Wheat, Cassava, Potatoes, and more
- **Real-time weather** — automatically fetches historical and seasonal weather data (rainfall and temperature) for the selected location via Open-Meteo
- **Yield prediction** — predicts crop yield using a Random Forest model trained on global agricultural data
- **Yield classification** — classifies the predicted yield as Good, Medium, or Bad relative to historical yields for that crop
- **Percentile ranking** — shows where the predicted yield stands relative to all historical yields for the selected crop

## How It Works

1. Select a location on the map or enter coordinates
2. Choose a crop type
3. Click **Predict** — the app fetches weather data for the current year and runs the prediction
4. View the predicted yield, yield category, rainfall, temperature, and percentile rank

## Tech Stack

- **Frontend** — HTML, CSS, JavaScript
- **Backend API** — Python, FastAPI, deployed on Azure App Service
- **ML Model** — Random Forest Regressor (scikit-learn)
- **Weather Data** — Open-Meteo Archive API and Seasonal Forecast API
