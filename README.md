# MNBC 2025 Seismic Hazard & Design Tool 🌍🏗️

A web-based geospatial application designed to help structural engineers and designers calculate seismic hazard parameters and determine the **Seismic Design Category (SDC)** based on the **Myanmar National Building Code (MNBC) 2025**.

## 📖 Overview

This tool provides an interactive map interface to quickly retrieve mapped spectral response acceleration parameters ($S_s$ and $S_1$) for any location in Myanmar. Based on the user-selected Site Class and Occupancy Category, the application automatically performs interpolations and calculates the design parameters to establish system limitations and structural irregularities.

## ✨ Key Features

* **Interactive Map:** Click anywhere on the map or search by coordinates (Lat, Lng) to instantly get site-specific $S_s$ and $S_1$ values.
* **Automated Calculations:** * Linear interpolation for Site Coefficients ($F_a$ and $F_v$).
  * Calculation of Design Spectral Acceleration Parameters ($S_{DS}$ and $S_{D1}$).
  * Automatic determination of the Seismic Design Category (SDC).
* **System Limitations Check:** Evaluates SFRS (Seismic Force-Resisting System) height limitations and structural irregularity penalties based on the calculated SDC.
* **PDF Report Generation:** One-click feature to generate and print a clean, formatted calculation report for documentation.
* **Fully Client-Side:** Runs entirely in the browser without needing a backend server.

## 🛠️ Technologies Used

* **HTML5, CSS3, Vanilla JavaScript**
* **[Leaflet.js](https://leafletjs.com/):** For interactive map rendering.
* **[Turf.js](https://turfjs.org/):** For advanced geospatial analysis (Point-in-Polygon calculations to extract GeoJSON data).

## 📂 Project Structure

```text
├── index.html       # Main application UI, styling, and core calculation logic
├── ss.js            # GeoJSON data for Short-Period Spectral Acceleration (Ss)
├── s1.js            # GeoJSON data for 1-Second Period Spectral Acceleration (S1)
└── README.md        # Project documentation
