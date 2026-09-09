# 🚗 Road Accident Analysis & Safety Dashboard

An interactive Power BI data analytics project evaluating 20,000 traffic accident records to identify high-risk areas, casualty patterns, and primary crash causes.

---

## 📌 Project Title
**Road Accident Severity and Risk Analysis Dashboard**

## 🎯 Project Objective
The objective of this project is to analyze historical road traffic accident data to identify high-risk zones, assess casualty patterns, and determine how factors such as driver behavior, road infrastructure, and weather conditions contribute to crash frequency and severity. The resulting Power BI dashboard enables interactive exploration to help traffic authorities and planners make data-driven safety decisions.

## 📂 Dataset Used
* **Dataset File**: [`road accident.csv`](https://github.com/prathiba076/Data-Analysis-Dashboard/blob/main/road%20accident.csv)
* **Power BI File**: [`road accident analysis.pbix`](https://github.com/prathiba076/Data-Analysis-Dashboard/blob/main/road%20accident%20analysis.pbix)
* **Key Attributes**:
  * **Location**: `city`, `state`, `latitude`, `longitude`
  * **Time & Date**: `date`, `time`, `hour`, `day_of_week`, `is_weekend`, `is_peak_hour`
  * **Road & Environment**: `road_type`, `lanes`, `traffic_signal`, `traffic_density`, `weather`, `visibility`, `temperature`
  * **Impact & Risk**: `cause`, `accident_severity` (fatal, major, minor), `vehicles_involved`, `casualties`, `risk_score`

---

## ❓ Business Questions Answered
1. **Total Impact**: What is the overall volume of accidents, total casualties, and vehicles involved?
2. **Crash Causes**: Which primary causes (overspeeding, drunk driving, distraction, weather, poor road conditions) result in the most fatal and major collisions?
3. **Temporal Trends**: Which hours of the day (peak vs. non-peak) and days of the week record the highest accident frequency?
4. **Weather Impact**: How strongly do poor weather conditions (rain, fog) and low visibility correlate with severe accidents?
5. **Road Infrastructure**: Does road design (highways vs. urban roads, number of lanes, presence of traffic signals) reduce or increase accident risk scores?
6. **Geographic Distribution**: Which cities and coordinates exhibit the greatest density of high-risk accidents?

---

## 🖥️ Dashboard Interaction
* **KPI Metric Cards**: Real-time totals for Total Accidents, Total Casualties, Vehicles Involved, and Average Risk Score.
* **Interactive Slicers**: Filter the report dynamically by City, Road Type, Weather Condition, Severity Level, and Date/Day.
* **Cross-Filtering**: Clicking any chart element instantly updates all connected visuals across the report.
* **Geospatial Hotspots**: Coordinate-based mapping visualization to explore location density and crash hotspots.
* **Drill-Down Capability**: Analyze accident frequency across days of the week down to individual hourly intervals.

---

## ⚙️ Process & Methodology
1. **Data Ingestion & Cleaning**:
   * Imported `road accident.csv` into Power BI via Power Query.
   * Standardized data types (coordinates as decimal, timestamps as date/time, categorical features as text).
   * Verified data completeness and handled missing values.
2. **Data Modeling & DAX Measures**:
   * Created custom measures for Total Accidents, Fatal Accident %, Total Casualties, and Average Risk Score.
3. **Exploratory Data Analysis (EDA)**:
   * Analyzed distribution across severity classes (`fatal`, `major`, `minor`).
   * Evaluated correlations between environmental factors, driver causes, and overall risk levels.
4. **Dashboard Layout & Design**:
   * Structured a visual hierarchy: top-level KPI scorecards, central distribution and geospatial visuals, and filter panels.
5. **Documentation & Publishing**:
   * Published project files and documentation to GitHub.

---

## 📁 Repository Structure
```text
Data-Analysis-Dashboard/
├── road accident.csv             # Raw source dataset
├── road accident analysis.pbix    # Power BI Dashboard report
└── README.md                     # Project documentation
