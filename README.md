# 🚗 Road Accident Analysis Dashboard | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-02569B?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=for-the-badge)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-4285F4?style=for-the-badge)

An interactive **Power BI dashboard** that analyzes over **308,000 road accidents** to identify accident trends, high-risk locations, contributing factors, and opportunities to improve road safety through data-driven decision-making.

---
# 📑 Table of Contents

- [Overview](#-overview)
- [Business Problem](#-business-problem)
- [Dataset Information](#-dataset-information)
- [Data Cleaning & Transformation](#-data-cleaning--transformation-power-query)
- [Data Modeling](#-data-modeling)
- [DAX Measures](#-dax-measures)
- [Dashboard Pages](#-dashboard-pages)
- [Key KPIs](#-key-kpis)
- [Business Insights](#-business-insights)
- [Business Recommendations](#-business-recommendations)
- [Dashboard Preview](#-dashboard-preview)
- [Skills Demonstrated](#-skills-demonstrated)
- [Repository Structure](#-repository-structure)
- [How to Use the Project](#-how-to-use-the-project)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---
# 📖 Overview

This project analyzes UK road accident data using **Power BI** to transform raw data into meaningful business insights. The dashboard provides an interactive view of accident trends, casualty statistics, vehicle involvement, environmental conditions, and geographic distribution.

The project covers the complete Business Intelligence workflow, including data cleaning, data modeling, DAX calculations, KPI development, and dashboard design.

The dashboard enables users to explore accident patterns, identify high-risk areas, and support data-driven road safety decisions.

---

# 🎯 Business Problem

Road accidents continue to cause injuries, fatalities, and significant economic losses every year. Transportation authorities require reliable insights to understand where accidents occur, when they happen most frequently, and which factors contribute to their severity.

The objective of this project is to transform raw accident data into an interactive dashboard that helps decision-makers identify accident trends and prioritize road safety improvements.

The dashboard answers questions such as:

- Which districts experience the highest number of accidents?
- When do accidents occur most frequently?
- Which vehicle types are most commonly involved?
- How do weather and road conditions affect accident severity?
- Which road types require additional safety measures?

---

# 📊 Dataset Information

**Dataset Source:** Kaggle

The dataset contains detailed information about road accidents, including:

- Accident Date
- Accident Severity
- Number of Casualties
- Number of Vehicles
- Vehicle Type
- Road Type
- Road Surface Conditions
- Weather Conditions
- Light Conditions
- Speed Limit
- Junction Control
- Carriageway Hazards
- Urban/Rural Area
- Police Force
- Local Authority District
- GPS Coordinates (Latitude & Longitude)

---

# 🧹 Data Cleaning & Transformation (Power Query)

The dataset was cleaned and prepared using **Power Query**.

### Data Cleaning Steps

- Verified data types
- Removed duplicate records using **Accident_Index**
- Checked for missing values
- Trimmed extra spaces
- Cleaned text fields
- Standardized text values
- Checked for invalid values
- Created a custom **Time of Day** column

### Time Categories

| Time | Category |
|-------|----------|
| 00:00 – 05:59 | Night |
| 06:00 – 11:59 | Morning |
| 12:00 – 17:59 | Afternoon |
| 18:00 – 23:59 | Evening |

---

# 🗂 Data Modeling

A Date Dimension (Dim_Date) table was created to support time intelligence analysis.

The Date Table includes:

- Date
- Year
- Quarter
- Month Number
- Month Name
- Day
- Day Name
- Day Number
- Month Year
- YearMonth

### Relationship

- One-to-Many (1:*)
- Single Cross Filter Direction
- Active Relationship

---

# 📐 DAX Measures

The project includes several DAX measures to calculate KPIs and create dynamic dashboard elements.

### KPI Measures

- Total Accidents
- Total Casualties
- Total Vehicles
- Fatal Accident %
- Serious Accident %
- Slight Accident %
- Urban Accidents
- Rural Accidents
- Districts with Accidents

### Dynamic Measures

- Selected Filter
- Dynamic Dashboard Titles
- Road Type Title
- Weather Title
- Road Surface Title
- Light Condition Title
- Junction Control Title
- Urban/Rural Title
- Carriageway Title

---

# 📈 Dashboard Pages

## 📄 Page 1 – Executive Summary

Features:

- KPI Cards
    - Total Accidents
    - Total Casualties
    - Total Vehicles
- Monthly Accident Trend
- Accident Severity Breakdown
- Top Districts
- Accident Location Map
- Interactive Slicers
    - Year
    - Month
    - District
- Dynamic Page Title

---

## 📄 Page 2 – Accident Analysis

Features:

- Accidents by Time of Day
- Accidents by Day of Week
- Accidents by Vehicle Type
- Accidents by Road Type
- Accidents by Speed Limit
- Interactive Slicers
- Dynamic Page Title

---

## 📄 Page 3 – Severity & Environmental Analysis

Features:

- Severity by Road Type
- Severity by Weather Conditions
- Severity by Light Conditions
- Severity by Road Surface Conditions
- Interactive Slicers
- Dynamic Page Title

---

## 📄 Page 4 – Geographic & Location Analysis

Features:

KPI Cards

- Total Districts
- Urban Accidents
- Rural Accidents

Visualizations

- Urban vs Rural Accident Distribution
- Accidents by Junction Control
- Accidents by Carriageway Hazards

Interactive Slicers

- Year
- Month
- District

Dynamic Page Title

---

# 📊 Key KPIs

| KPI | Value |
|------|-------|
| Total Accidents | 308K+ |
| Total Casualties | 418K+ |
| Total Vehicles | 563K+ |
| Districts Covered | 417 |
| Fatal Accidents | 1.28% |

---

# 💡 Business Insights

## Executive Summary

- Over **308,000 accidents** resulted in **418,000+ casualties** involving more than **563,000 vehicles**.
- Birmingham recorded the highest number of accidents, followed by Leeds and Manchester.
- Accident frequency remained relatively stable throughout the year with slight declines during February and December 2022.
- Approximately **85%** of accidents were classified as Slight, while Fatal accidents accounted for only **1.28%**.

## Accident Analysis

- Most accidents occurred during the afternoon.
- Saturdays experienced the highest accident frequency.
- Passenger cars were involved in the majority of accidents.
- Single carriageways recorded the highest accident count.
- Roads with a 30 mph speed limit experienced the largest number of accidents.

## Severity & Environmental Analysis

- Most accidents occurred during good weather and daylight conditions.
- Dry road surfaces recorded the highest number of accidents.
- Single carriageways experienced the highest number of serious and fatal accidents.
- Traffic volume appears to have a greater influence on accident frequency than adverse weather conditions.

## Geographic Analysis

- Approximately 64% of accidents occurred in urban areas.
- Give-way and uncontrolled junctions experienced the highest accident frequency.
- Road debris was the most common carriageway hazard.
- The dataset covers 417 districts across the UK.

---

# ✅ Business Recommendations

- Prioritize road safety improvements in Birmingham, Leeds, and Manchester.
- Increase traffic enforcement during afternoon peak hours and weekends.
- Improve pedestrian crossings and traffic calming measures on 30 mph roads.
- Upgrade uncontrolled junctions with improved signage and visibility.
- Enhance safety measures on single carriageways.
- Continue maintaining road surfaces and rapidly remove carriageway hazards.
- Monitor accident hotspots continuously using data-driven analysis.

---

# 🖼 Dashboard Preview

## Executive Summary

<img width="1157" height="662" alt="Screenshot 2026-07-05 014959" src="https://github.com/user-attachments/assets/a82fbfeb-1cd3-4714-ad88-65dff3d9f8c7" />


## Accident Analysis

<img width="1157" height="666" alt="Screenshot 2026-07-05 212350" src="https://github.com/user-attachments/assets/42667655-58ec-487f-83d0-361f0274d1d1" />


## Severity & Environmental Analysis

<img width="1136" height="737" alt="Screenshot 2026-07-05 212927" src="https://github.com/user-attachments/assets/ba1f27ba-76f3-4638-9224-8569557d4750" />


## Geographic & Location Analysis

<img width="1158" height="652" alt="Screenshot 2026-07-05 214640" src="https://github.com/user-attachments/assets/bbfacb70-5b2f-4b19-ad6b-a1a53eeb84ff" />


---

# 🛠 Skills Demonstrated

### Data Preparation

- Power Query
- Data Cleaning
- Data Validation
- Data Transformation
- Handling Missing Values

### Data Modeling

- Star Schema Design
- Date Dimension Creation
- Relationship Management

### DAX

- Measures
- KPIs
- Percentage Calculations
- Dynamic Titles
- Interactive Filtering

### Dashboard Development

- Interactive Dashboards
- KPI Cards
- Maps
- Slicers
- Business Storytelling
- Data Visualization

### Business Analysis

- Trend Analysis
- Geographic Analysis
- Severity Analysis
- Business Insights
- Data-Driven Recommendations

---

# 📁 Repository Structure

```
Road-Accident-Analysis-PowerBI/
│
├── README.md
├── Road Accident Dashboard.pbix
├── Road_Accident_Data.xlsx
└── screenshots/
    ├── Executive Summary.png
    ├── Accident Analysis.png
    ├── Severity Analysis.png
    └── Geographic Analysis.png
```

---

# 🚀 How to Use the Project

1. Clone or download this repository.
2. Open **Road Accident Dashboard.pbix** using **Power BI Desktop**.
3. Load the dataset if prompted.
4. Explore the dashboard using the interactive slicers.
5. Navigate through the four dashboard pages.
6. Interact with charts, maps, and KPIs to explore accident trends and insights.

---

# 🔮 Future Improvements

Possible enhancements include:

- Integrating live accident data using APIs.
- Developing predictive accident risk models with Machine Learning.
- Adding drill-through pages for district-level analysis.
- Implementing forecasting for future accident trends.
- Optimizing the dashboard for mobile devices.
- Publishing the dashboard to Power BI Service for online sharing.

---

# 👤 Author

**Alaa Kanaan**

Aspiring Data Analyst passionate about transforming data into meaningful insights through **Power BI, SQL, Excel, Python, and Data Visualization**.

If you found this project helpful or have any feedback, feel free to connect with me on LinkedIn or explore my other projects on GitHub.

---

⭐ If you found this project useful, consider giving this repository a **Star** on GitHub!
