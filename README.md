# 2026 YTD Chicago Travel Safety Index: Public Street Crime Assessment

A data-driven geospatial analysis and visualization project assessing public safety across Chicago's community areas. This project utilizes automated API ingestion and local demographic data to calculate crime rates per 10,000 population, providing clear, actionable insights for travelers and city planners.

![Chicago Safety Index](chicago.jpg)

---

## 📌 Project Overview
This project examines public incident data—specifically targeting high-impact street crimes such as **Theft, Robbery, and Assault**—from January to June 2026. By merging real-time geospatial boundaries with localized population statistics, the pipeline generates dual-aligned visualizations detailing the top 10 highest-risk neighborhoods alongside a spatial distribution choropleth map.

### Key Features
* **Dynamic API Integration:** Real-time fetching of Chicago Community Area geometric boundaries (GeoJSON/MultiPolygon) directly from the Chicago Data Portal API.
* **Geospatial Processing:** Converts raw API dictionary formats into active `shapely` geometric objects for zero-latency spatial plotting.
* **Professional Dual-Layout Data Visualization:** Side-by-side synchronized rendering of a Top 10 horizontal bar chart and a highly detailed, non-overlapping labeled choropleth map with customized alignment for complex areas (e.g., The Loop, O'Hare).

---

## 📁 Repository Structure

```text
├── .env.example                         # Environment variables template for API credentials
├── chicago.jpg                          # Cover/Banner visual asset for the repository
├── crime.ipynb                          # Master Jupyter Notebook containing ETL, EDA, and Plotting
├── dataset_sample.csv                   # Sample dataset (100 rows) for structural reference
└── population_by_community_area_2025.csv # Core local demographic reference dataset
