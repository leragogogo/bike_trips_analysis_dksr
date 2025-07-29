# Bike Trips Analysis

This project analyzes bike trip data using Python and visualizes spatial and temporal patterns with heatmaps and line plots. 
It reveals patterns in route usage by **hour of day**, **day of the week**, and overall **trip density**.

## Features

### Data Consistency Checks
- **Spatial consistency**: verified that all trips are located in and around one city (Mainz), allowing for Euclidean interpolation.
- **Temporal consistency**: time intervals between sensor readings are mostly regular (under 10 minutes in 99.98% cases).

### Heatmaps
- **Panel + Datashader heatmap**: lightweight and efficient rendering of millions of interpolated points on OpenStreetMap.
- **Heatmap by weekday**: animated map using `HeatMapWithTime`.
- **Heatmap by hour**: aggregated route activity by time of day.

### Line Charts
- Trip distribution by **hour of day** and **weekday** to identify peak usage times.

## Technologies Used

- `pandas`, `numpy`, `matplotlib`
- `folium`, `HeatMap`, `HeatMapWithTime` for interactive mapping
