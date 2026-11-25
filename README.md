# Heatwave-Safe Pedestrian Routing Algorithm Using Public GIS and Real-Time Meteorological Data

> **Presented at the 2026 KISM (Korea Institute of Smart Media) Spring Conference**  
> A pedestrian graph-routing algorithm that integrates public GIS walkway networks with real-time meteorological observations to minimize heat-stress exposure during extreme heat events.

---

## Overview & Motivation
- Conventional pedestrian navigation optimizes strictly for shortest distance or minimum travel time, often routing pedestrians through unshaded, high-radiant-heat corridors during heatwaves.
- This project maps real-time meteorological variables (ambient temperature, humidity, and apparent temperature) onto public GIS pedestrian road networks to compute composite thermal-risk edge weights and generate safer walking routes.

## Core Implementation
1. **GIS Pedestrian Network Modeling:** Constructed a directed node-edge graph from public spatial pedestrian road datasets.
2. **Real-Time Meteorological Spatial Mapping:** Fetched live weather observations via public meteorological APIs and interpolated thermal-stress indices across road segments.
3. **Thermal-Aware Pathfinding:** Implemented a multi-objective cost function balancing physical distance and thermal-exposure penalties to reduce cumulative heat load compared to shortest-path baselines.

## Tech Stack
- **Language:** Python 3
- **Data & Spatial Processing:** Pandas, NumPy, GIS / Graph Routing Libraries
- **Data Sources:** Public GIS Pedestrian Road Network Data, Real-Time Meteorological Observation API

## Getting Started
1. Clone this repository and install dependencies (`pip install -r requirements.txt`).
2. Create a `.env` file in the root directory and configure your meteorological API key.
3. Run the routing pipeline (`python main.py`) to compare shortest vs. heatwave-safe pedestrian paths.

## Publication
- **2026 KISM Spring Conference:** Authored and presented research paper on heatwave-safe pedestrian routing using GIS and real-time weather data.
