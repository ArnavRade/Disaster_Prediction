# AI-Driven City Scale Casualty & Impact Prediction Engine

An AI-powered disaster intelligence platform that predicts the impact and risk zones of disasters at a city scale using machine learning, geospatial analysis, and grid-based landscape modeling.
The system divides a city into hierarchical spatial grids, analyzes environmental and human-induced risk factors, and predicts disaster impact severity in each zone.

Formerly implemented for Guwahati, currently implemented for any city, focusing on:
Earthquakes
Landslides

The platform provides a visual risk heatmap and prediction dashboard to assist emergency response teams, urban planners, and disaster management authorities.

1. Project Vision

Natural disasters cause significant casualties due to lack of localized prediction systems.
Most current systems:
Predict disasters globally
Do not estimate city-scale impact
Ignore human-induced risk factors

This project solves that by creating a city-level AI engine that predicts how disasters affect different zones differently.

2.  Core Idea

The city is divided into multi-level spatial grids.

City
 ├── Primary Grid (Lat-Long Segmentation)
 │      ├── Sub-Grid Matrix
 │      │      ├── Landscape Weight Assignment
 │      │      └── Event Risk Modeling

Each grid is analyzed based on:
Terrain
Disaster history
Environmental features
Human activities

An AI model predicts disaster impact for each grid cell.

3. System Architecture
   
Frontend Dashboard
        ↓
Prediction API
        ↓
Grid-Based Spatial Engine
        ↓
XGBoost Machine Learning Model
        ↓
Disaster Risk Prediction
        ↓
Interactive Risk Heatmap

4.  Tech Stack
   
Frontend -
React
TailwindCSS
Leaflet / Mapbox
Interactive Grid Heatmaps

Backend - 
FastAPI
Python
REST APIs

Machine Learning - 
XGBoost

Libraries used - 
Scikit-Learn
Pandas
NumPy
Geospatial Processing
GeoPandas
Shapely

5. AI Integration
OpenAI API (for explanation and disaster insights)

6. Datasets Used
Global datasets filtered for Guwahati using latitude and longitude.

Earthquake Dataset - 
Includes: Magnitude, Depth, Location, Time, Error margins

Landslide Dataset - 
Includes: Event category, Trigger, Landslide size, Location description, Event timestamp

7. Key Features
  I) Grid-Based Risk Mapping
  II) The city is divided into multi-level spatial grids allowing fine-grained disaster impact prediction.
  III) AI-Driven Impact Prediction
  IV) Landscape-Aware Risk Weighting

Each grid cell receives weights based on:
> river proximity
> hills and slopes
> vegetation density
> terrain characteristics

Human Activity Risk Simulation
The system considers man-made factors like:
> tunnel construction
> mining or blasting
> deforestation
> heavy infrastructure development
> war/bombing events (simulated)
These activities dynamically increase disaster probability in affected grids.


8. Unique Selling Points (USPs) -
   
1️⃣ City-Scale Disaster Intelligence
Unlike global prediction models, this system works at city resolution.

2️⃣ Hierarchical Grid Architecture
Multi-level segmentation enables precise spatial risk modeling.

3️⃣ Human Activity Integration
Most disaster systems ignore anthropogenic triggers. This platform dynamically models human-induced risks.

4️⃣ Real-Time Risk Simulation
Users can simulate activities such as:
> tunnel digging
> deforestation
> infrastructure projects
> instantly see risk propagation across grids.

5️⃣ AI-Explainable Predictions
Integration with AI models provides human-readable explanations for predicted risk levels.

9. Sustainable Development Goals (SDG) Alignment

  I. SDG 11 — Sustainable Cities and Communities
  II. SDG 13 — Climate Action
  III. SDG 9 — Industry, Innovation and Infrastructure
  IV. SDG 3 — Good Health and Well-Being

10. Future Enhancements - 
Flood modeling
Wildfire spread prediction
Reinforcement learning for adaptive risk modeling
IoT sensor integration for live monitoring
