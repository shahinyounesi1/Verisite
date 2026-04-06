# ☀️ Verisite: Solar Land Viability Assessment (GIS Data Pipeline)

![Verisite GIS Map](images/main-map.png)

## 📌 Overview
Verisite is a spatial intelligence data pipeline designed to accelerate the preliminary Due Diligence phase for utility-scale solar energy development in the UK. 

Currently in its core database development phase (MVP), this project automates the identification, filtering, and assessment of optimal land parcels by integrating complex UK urban planning regulations, environmental constraints, and electrical grid infrastructure data.

## 🎯 The Problem
Finding developable land for renewable energy projects involves navigating a labyrinth of spatial constraints. Developers often waste significant time assessing plots that are ultimately unviable due to hidden planning restrictions (e.g., Green Belt policies) or excessive distance from grid connection points.

## 💡 Methodology & Data Engineering
This repository contains the robust GIS data pipeline built to filter and score land parcels in Northumberland. The workflow includes:

1.  **Constraint Mapping (Restricted Zones):** Aggregation and integration of "No-Go" layers including:
    * Green Belt and AONB (Area of Outstanding Natural Beauty)
    * Flood Zones (Environment Agency data)
    * Scheduled Monuments and Heritage Sites
    * Agricultural Land Classifications
2.  **Viability Extraction (Verified Zones):** Utilizing advanced spatial operations (Difference algorithms, Multipart geometry standardization) to extract pristine, developable land parcels.
3.  **Grid Proximity Engine:** Calculating exact distances from verified land parcels to the nearest National Grid substations using nearest-neighbor spatial joins, categorizing them into commercial viability zones (e.g., 0-2 km, 2-10 km).
4.  **Database Optimization:** Compiling the processed data into a clean, lightweight GeoJSON format, ready for future web-map integration.

## 🛠️ Tech Stack & Skills Demonstrated
* **Geospatial Analysis:** QGIS, Vector geometry processing.
* **Database Management:** Spatial SQL (Field Calculator), GeoPackage, GeoJSON.
* **Domain Expertise:** UK Town and Country Planning regulations, Renewable Energy infrastructure planning.

## 📁 Repository Structure
* `/data`: Contains the finalized `Verisite_WebMap.geojson` file with all calculated attributes (Status, Grid_Zone, distance).
* `/images`: Visual documentation of the GIS processing steps and final outputs.

## 👨‍💻 About the Developer
Developed by an Urban Planning Master's student and Chevening Scholar based at Newcastle University. This project bridges the gap between academic urban theory and practical, tech-driven solutions for real-world environmental challenges. 

*Let's connect!*
🔗 [My LinkedIn Profile](Link-to-your-LinkedIn)
