# ☀️ Verisite: Solar Land Viability Assessment Platform (MVP)

![Verisite Web Interface](link-to-your-screenshot-here.png)

## 📌 Overview
Verisite is a PropTech/ClimateTech Proof of Concept (PoC) designed to accelerate the transition to Net-Zero in the UK. It is a spatial intelligence platform that automates the identification and assessment of optimal land parcels for utility-scale solar energy development. 

By integrating complex UK urban planning constraints, environmental restrictions, and electrical grid infrastructure data, Verisite reduces the preliminary Due Diligence phase for solar developers from weeks to minutes.

## 🎯 The Problem
Finding suitable land for renewable energy projects in the UK involves navigating a labyrinth of spatial constraints. Developers often waste significant time and capital assessing plots that are ultimately unviable due to hidden planning restrictions (e.g., Green Belt policies) or excessive distance from grid connection points.

## 💡 The Solution (Methodology)
This project utilizes a robust GIS data pipeline to filter and score land parcels in Northumberland. The methodology includes:

1.  **Constraint Mapping (The "Red Zones"):** Aggregation and integration of restrictive layers including:
    * Green Belt and AONB (Area of Outstanding Natural Beauty)
    * Flood Zones (Environment Agency data)
    * Scheduled Monuments and Heritage Sites
    * Agricultural Land Classifications
2.  **Viability Extraction (The "Green Zones"):** Utilizing advanced spatial operations (Difference algorithms, Multipart geometry standardization) to extract pristine, developable land parcels.
3.  **Grid Proximity Engine:** Calculating exact distances from verified land parcels to the nearest National Grid substations using nearest-neighbor spatial joins, categorizing them into commercial viability zones (e.g., 0-2 km, 2-10 km).
4.  **Web Visualization:** Exporting the optimized database into a lightweight GeoJSON format, rendered through a custom, interactive web map interface.

## 🛠️ Tech Stack & Skills Demonstrated
* **Spatial Analysis & Database Management:** QGIS, GeoPackage, Spatial SQL, Geometry standardization.
* **Front-End Web Development:** HTML5, CSS3, JavaScript.
* **Web Mapping Library:** Leaflet.js (Custom Dark Mode UI, dynamic pop-ups, GeoJSON rendering).
* **Domain Expertise:** UK Town and Country Planning regulations, Renewable Energy infrastructure planning.

## 🚀 How to Run the MVP Locally
1. Clone this repository: `git clone https://github.com/YourUsername/verisite.git`
2. Open the project folder.
3. Simply double-click the `index.html` file to launch the interactive web map in your browser (No local server or API keys required).
4. Click on any colored parcel to view its specific development status, grid zone, and exact distance to the nearest substation.

## 🔮 Future Roadmap (Next Iterations)
* Integration of DEM (Digital Elevation Model) data for automated slope and aspect analysis.
* Solar irradiance modeling for financial forecasting.
* API integration with HM Land Registry for ownership insights.

## 👨‍💻 About the Developer
Developed by an Urban Planning Master's student and Chevening Scholar based at Newcastle University. This project bridges the gap between academic urban theory and practical, tech-driven solutions for real-world environmental challenges. 

*Let's connect!*
🔗 [My LinkedIn Profile](Link-to-your-LinkedIn)
