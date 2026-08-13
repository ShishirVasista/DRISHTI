# DRISTI 🌊

### Disaster Risk Intelligence System for Hazard Tracking & Impact

DRISTI is an AI-powered disaster response system that predicts flood risk and optimizes emergency resource allocation for at-risk communities. By combining geospatial analysis, machine learning, and optimization algorithms, DRISTI analyzes rainfall forecasts, elevation data, population density, and historical disaster patterns to identify vulnerable zones **before** a crisis unfolds — and recommends how to respond once it does.

> *Dristi (दृष्टि) — Sanskrit for "vision" or "foresight." The name reflects the system's core purpose: seeing disaster risk before it happens.*

---

## What It Does

When heavy rainfall is predicted for a region, DRISTI automatically:

1. **Predicts flood risk** across zones using elevation, rainfall, and historical flood data
2. **Identifies vulnerable populations** by overlaying risk zones with population density data
3. **Forecasts rainfall timing** to estimate when flooding will peak
4. **Maps road network disruptions** to flag impassable routes and suggest evacuation paths
5. **Optimizes resource allocation** — distributing limited rescue teams, medical units, and supplies across affected zones to minimize response time
6. **Generates an authority-ready report** with risk maps, affected population estimates, and a recommended action plan

---

## Tech Stack

| Layer | Tools |
|---|---|
| Geospatial processing | GeoPandas, Rasterio |
| Risk prediction | Scikit-learn, XGBoost |
| Forecasting | Prophet / ARIMA (statsmodels) |
| Road network analysis | NetworkX, OSMnx |
| Resource optimization | PuLP |
| Visualization | Folium |
| Backend | FastAPI |
| Frontend | Streamlit |
| Database | SQLite / PostGIS |

---

## Data Sources

- **Elevation (DEM):** USGS / SRTM (earthexplorer.usgs.gov)
- **Rainfall & weather:** Open-Meteo API
- **Population density:** WorldPop / CIESIN
- **Road networks:** OpenStreetMap (via OSMnx)
- **Historical disasters:** NDRF, government reports

---

## Project Structure

```
dristi/
├── src/
│   ├── risk/           # Flood risk prediction model
│   ├── geo/             # Elevation & population impact analysis
│   ├── optimization/    # Resource allocation solver
│   ├── network/         # Road network & evacuation routing
│   └── api/              # FastAPI backend
├── app/                  # Streamlit dashboard
├── data/                 # Datasets (raw & processed)
├── notebooks/            # Exploratory analysis
├── tests/
├── requirements.txt
└── README.md
```

---

## Team

| Member | Module |
|---|---|
| — | Risk Prediction & Forecasting |
| — | Geospatial Analysis & Population Impact |
| — | Optimization & Road Network Analysis |
| — | Backend, Integration & Frontend |

---

## Status

🚧 In development — college final year project.
