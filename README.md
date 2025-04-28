# Land Insight AI: Smart Land Monitoring System

**A modern, tech-themed approach to land management for urban planning, government, and sustainability.** [cite: 1]

## Project Description

Land Insight AI is a system designed to digitize, analyze, and visualize land data to improve decision-making in urban planning and land management. [cite: 13, 2, 3] It addresses the inefficiencies and inaccuracies of traditional manual land record systems. [cite: 12]

## Objectives

* **Centralize Land Data Digitally:** Consolidate land-related information into a digital format. [cite: 3]
* **Enable Smart Price Analytics:** Provide tools for analyzing land prices. [cite: 3]
* **Visualize Land Distribution and Pricing:** Offer visual representations of land data through interactive maps. [cite: 3]
* **Enhance Stakeholder Decision Making:** Support better-informed decisions by government, investors, and developers. [cite: 3, 28]

## Key Features

* **Interactive Maps:** Folium-based maps displaying land parcels, price heatmaps, and analysis overlays. [cite: 7, 40]
* **Smart Price Analytics:** Analysis of land prices, including average prices and zone-specific averages. [cite: 3, 14]
* **City Selection:** User-friendly interface with a dropdown menu to select cities. [cite: 7]
* **Land Data Management:** System for loading, saving, and processing land data. [cite: 3]
* **Distance Calculation:** Implementation of the Haversine formula to calculate distances and identify properties within a specified radius. [cite: 6]
* **GUI (Graphical User Interface):** Tkinter-based GUI for user interaction. [cite: 7]

## Architecture

The system is structured with the following layers:

* **Frontend:** Tkinter-based GUI (`MAIN_GUI.PY`) for user interaction (city selection, analyzing prices, generating/exploring maps). [cite: 3]
* **Core Logic Layer:** Python module (`INDIA_LAND_SYSTEM.PY`) containing the core functionalities:
    * Data loading and saving. [cite: 3]
    * Price analysis. [cite: 3]
    * Property classification. [cite: 3]
    * Geocoding. [cite: 3]
    * Map generation. [cite: 3]
* **Data Storage:** JSON file (`india_land_data.json`) for storing land data. [cite: 3, 40]
* **Visualization Layer:** HTML file (`LAND_MAP.HTML`) utilizing Folium and Leaflet for map rendering. [cite: 3]

## Methodology

1.  **Land Data Generation and Preprocessing:**
    * Uses simulated or real datasets with attributes like latitude, longitude, zone, classification, area, and price. [cite: 4, 5]
    * Includes data cleaning, formatting, and unit normalization. [cite: 4, 5]

2.  **Distance Calculation:**
    * Employs the Haversine formula to calculate distances between land parcels. [cite: 6]
    * Filters properties based on proximity to a selected city (e.g., within a 30 km radius). [cite: 6, 40]

3.  **Land Price Analysis:**
    * Uses a heap-based algorithm to find the K cheapest and K most expensive land parcels. [cite: 7]
    * Currently uses rule-based logic for initial price calculation (can be replaced with ML models). [cite: 39]

4.  **Interactive Map Visualization:**
    * Generates interactive maps with:
        * Color-coded markers to represent land classifications. [cite: 7, 40]
        * Price heatmaps. [cite: 7, 40]
        * Popups with detailed land information. [cite: 40]

## Technologies Used

* Python
* Tkinter (for GUI) [cite: 7, 25]
* Folium (for map visualization) [cite: 7, 40]
* Leaflet (for map rendering) [cite: 3]
* NumPy (for numerical operations) [cite: 8]
* JSON (for data storage) [cite: 8, 40]
* geopy (for geocoding) [cite: 8]
* heapq (for heap-based search) [cite: 7]

## Installation

1.  Clone the repository.
2.  Ensure you have Python installed.
3.  Install the required Python libraries (e.g., `folium`, `tkinter`, `numpy`, `geopy`). You can use `pip` for this:
    ```bash
    pip install folium numpy geopy
    # ... any other libraries
    ```
4.  Run the main Python script (`MAIN_GUI.PY`).

##  Sample Usage

1.  Select a city from the dropdown menu.
2.  Click the "Analyze Prices" button to view price statistics.
3.  Click "Generate Map" to see the interactive map.
4.  Use "Explore Location (Click Mode)" to click on map locations and see details.

##  Results

The system provides:

* Average land prices for a selected city. [cite: 14]
* Average land prices by zone within the city. [cite: 14]
* Interactive map visualization of land parcels with detailed information. [cite: 15, 16, 17]

The analysis helps to understand land price variations based on location, zone, and classification. [cite: 18, 19, 20, 21]

##  Future Enhancements

* Integration of machine learning models for more accurate price prediction. [cite: 9, 39]
* Expansion to include more cities and data sources.
* Development of a web-based application.
* Real-time data updates.

* Ishan Yadav (RA2311026010130) [cite: 2]


##  References

* [https://www.zillow.com/tech/](https://www.zillow.com/tech/) [cite: 25]
* [https://wiki.openstreetmap.org/](https://wiki.openstreetmap.org/) [cite: 25]
* [https://ai.googleblog.com/](https://ai.googleblog.com/) [cite: 25]
