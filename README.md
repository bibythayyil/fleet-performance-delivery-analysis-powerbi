# Fleet Performance & Delivery Efficiency Dashboard

> An AI-powered Power BI dashboard analyzing fleet trip performance, fuel efficiency, on-time delivery rates, and cost per km for a logistics company — built as a module end assignment for the Data Analytics course.

---

<p align="center">
  <img src="https://raw.githubusercontent.com/bibythayyil/bibythayyil/main/assets/fleet_performance_dashboard.png" width="900">
</p>

---

## Project Overview

A logistics company wanted to analyze its fleet performance in terms of on-time deliveries, fuel efficiency, and cost per kilometre. This project builds an interactive Power BI dashboard using trip and vehicle data, incorporating DAX measures and AI-powered visuals to uncover operational insights and support route and fleet optimization decisions.

---

## Dashboard Preview

![Fleet Performance Dashboard](Dashboard.pdf)

> Open `Dashboard.pdf` for a full visual preview of the dashboard without downloading Power BI.

---

## Dataset

**File:** `logistics_project_dataset.xlsx`

| Sheet | Records | Description |
|---|---|---|
| Trip_Data | 50 trips | Trip ID, Vehicle ID, Driver ID, Origin, Destination, Distance (km), Fuel Consumed (L), Delivery Status, Delivery Date |
| Vehicle_Master | 7 vehicles | Vehicle ID, Vehicle Type (Van, Truck, Mini-Truck), Capacity (kg), Maintenance Cost |

### Delivery Status Summary

| Status | Count |
|---|---|
| On-Time | 30 (60%) |
| Late | 20 (40%) |

---

## Project Tasks

### 1. Data Cleaning & Modeling
- Fixed missing fuel consumption values using mean imputation
- Created a relationship between Trip_Data and Vehicle_Master tables using Vehicle_ID

### 2. DAX Measures

| Measure | Formula |
|---|---|
| Fuel Efficiency | Distance / Fuel Consumed |
| On-Time Delivery % | On-Time Trips / Total Trips |
| Cost per km | (Fuel Cost + Maintenance Cost) / Distance |

> Fuel cost assumed at ₹100 per litre as per assignment specification

### 3. Visualizations

| Visual Type | Description |
|---|---|
| Bar Chart | On-Time Delivery % by Destination |
| Line Chart | Fuel Efficiency trend by Delivery Date |
| Card | Average Delivery Time |
| Card | Average Cost per km |
| Pie Chart | Vehicle Type vs Average Maintenance Cost |

### 4. AI-Powered Visuals

| Visual | Configuration |
|---|---|
| Q&A Visual | Prompt: "Average Cost per km by vehicle type?" |
| Key Influencers | Analyze: Delivery Status — Explained by: Distance (km), Vehicle Type, Driver ID |
| Decomposition Tree | Analyze: Cost per km — Explained by: Vehicle Type, Maintenance Cost, Distance (km) |

---

## Files in This Repository

| File | Description |
|---|---|
| `Fleet_Performance_and_Delivery_Efficiency.pbix` | Power BI dashboard file |
| `logistics_project_dataset.xlsx` | Source dataset (Trip_Data and Vehicle_Master sheets) |
| `Dashboard.pdf` | Dashboard visual preview |
| `README.md` | Project documentation |

---

## How to Use

1. Clone or download this repository
```bash
git clone https://github.com/bibythayyil/fleet-performance-delivery-analysis-powerbi
```

2. For a quick preview — open `Dashboard.pdf`

3. For the full interactive dashboard — open `Fleet_Performance_and_Delivery_Efficiency.pbix` in **Microsoft Power BI Desktop**

4. If prompted to refresh data, update the source path to point to `logistics_project_dataset.xlsx` on your local machine

5. Explore the dashboard pages for fleet performance and delivery insights

> **Note:** Power BI Desktop is free to download from [Microsoft](https://powerbi.microsoft.com/desktop/). AI-powered visuals (Key Influencers, Decomposition Tree) require a Power BI account sign-in.

---

## Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard development and visualization |
| Power Query | Data cleaning and transformation |
| DAX | Calculated measures and KPIs |
| AI Visuals | Q&A, Key Influencers, Decomposition Tree |
| Microsoft Excel | Source dataset |

---

## Author

**Bibin T S**

---
