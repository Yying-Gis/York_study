# York Community Resources WebGIS

## Overview
This project is a **learning-oriented WebGIS dashboard** developed from Python analysis in Google Colab.  
It demonstrates how to integrate **open datasets** with **Leaflet.js** to build an interactive web-based tool for exploring community resources in York.  
The work is for **educational purposes only** and **not for commercial use**.

------

## Background
- The main web interface (`index.html`) is adapted from outputs generated in **Google Colab**.  
  Reference version available in Google Drive: *(https://colab.research.google.com/drive/1nlhcaIYpJJqZtaqbkJTr_GGp0yd-XbNC?usp=sharing)*  
- Website uses **Leaflet.js** for the base map.  
- **GeoJSON files** (prepared in Google Drive: https://drive.google.com/drive/folders/1Si3aQVydmqm-jUbQ5HrfG4nMCsk4eRFE?usp=sharing) are used to provide dashboard content.  
- The dashboard includes **population distribution pie charts**.  
- Travel time calculations are simplified due to limited resources:  
  - Fixed **origin point** = York Railway Station  
  - Destination = selected **facility points** only  
  - This ensures smooth performance on a lightweight web server.  
- Different age groups use different facilities; therefore, data is combined in one platform to support analysis and planning.  

------

## Key Features
-  **Population Distribution**: Ward-level pie charts showing age group structures, allowing comparison of population proportions across wards  
-  **Community Facilities**: Facility layers (healthcare, schools, libraries, infrastructure) to compare whether resources are sufficiently distributed across wards  
-  **Travel Time Estimation**: Pre-calculated accessibility from York Railway Station to facilities, optimized for performance  
-  **Interactive Mapping**: Leaflet-based dashboard with layer toggles, charts, and combined demographic + facility data for analysis and planning

------

## Tech Stack
- **Python** (GeoPandas, Folium, OSMnx, Pandas) for geospatial data processing in Google Colab  
- **Leaflet.js** for interactive web mapping  (* openstreetmap)
- **HTML / JavaScript / CSS** for dashboard interface and KPI-style cards  
- **GeoJSON** for geospatial data storage and visualization  
- **Flask (app.py)** to serve the web application and API endpoints  
- **API Integration** for dynamic data handling and interaction  
- **Render** for cloud deployment and hosting of the WebGIS dashboard  
- **Google Colab + Google Drive** for workflow, preprocessing, and data storage

------

## Disclaimer
- This project is for **practice and learning purposes only**.  
- All datasets are sourced from **open data platforms** and **official government portals**.  
- Data ownership and rights remain with the original providers.

------

## How to Use
1. Open `index.html` in a browser to explore the interactive dashboard.  
2. Layers and charts can be toggled on/off for different facility categories.  
3. Refer to the Google Drive link for raw GeoJSON files and the original Colab notebook.  
