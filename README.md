# UK Road Accident Analysis Dashboard

## Project Overview

This project analyzes road accident data across the United Kingdom using Microsoft Power BI. The goal of the report is to identify patterns, trends, and risk factors associated with road accidents and present the findings through an interactive dashboard.

The dashboard enables stakeholders, analysts, and decision-makers to explore accident statistics by:

* Region and country
* Accident severity
* Road and weather conditions
* Driver demographics
* Vehicle types
* Time and location trends
* Casualties and accident costs

The project combines raw accident data with interactive visual analytics to support data-driven insights into road safety and transportation planning.

---

# Project Objectives

The primary objectives of this analysis are:

1. Identify regions with the highest number of road accidents.
2. Analyze accident severity distribution across the UK.
3. Understand the relationship between road conditions and accident occurrence.
4. Evaluate driver demographics involved in accidents.
5. Identify vehicle categories most frequently associated with accidents.
6. Explore temporal trends such as peak accident periods.
7. Estimate the economic impact of road accidents using accidental cost metrics.
8. Build an interactive Power BI dashboard for dynamic exploration and reporting.

---

# Dataset Information

## Source Files

### Raw Dataset

* **File Name:** `UK Accident Information (Data Import).xlsx`
* **Format:** Microsoft Excel Workbook

### Power BI Dashboard

* **File Name:** `Accident Report.pbix`
* **Format:** Microsoft Power BI Report

---

# Dataset Description

The dataset contains road accident records and related information for locations across the United Kingdom.

## Dataset Fields

| Column Name          | Description                                 |
| -------------------- | ------------------------------------------- |
| ID                   | Unique identifier for each accident record  |
| Date                 | Date of the accident                        |
| Location ID          | Unique identifier for the accident location |
| Location Description | Description of the accident location        |
| Region               | UK region where the accident occurred       |
| Country              | Country within the UK                       |
| Latitude             | Geographic latitude coordinate              |
| Longitude            | Geographic longitude coordinate             |
| Area Type            | Urban or rural classification               |
| Junction Control     | Traffic control type at the junction        |
| Accident Severity    | Severity classification of the accident     |
| Time of Day          | Time category when the accident occurred    |
| Road Conditions      | Road surface or weather-related conditions  |
| Junction Detail      | Junction structure or layout information    |
| Driver Age           | Age of the driver involved                  |
| Sex of Driver        | Gender of the driver                        |
| Vehicle Type         | Type of vehicle involved                    |
| Vehicle Propulsion   | Vehicle propulsion or fuel type             |
| Number of Accidents  | Total accident count                        |
| Number of Casualties | Total casualties reported                   |
| Number of Vehicles   | Number of vehicles involved                 |
| Accidental Costs     | Estimated economic cost of the accident     |

---

# Tools & Technologies

## Data Analysis

* Microsoft Excel
* Power BI Desktop

## Visualization

* Interactive dashboards
* Maps and geographic visuals
* KPI cards
* Trend analysis charts
* Slicers and filters

---

# Dashboard Features

The Power BI dashboard provides:

## Key Performance Indicators (KPIs)

* Total accidents
* Total casualties
* Total vehicles involved
* Total accident costs

## Interactive Filtering

Users can filter the dashboard by:

* Region
* Country
* Accident severity
* Vehicle type
* Driver gender
* Area type
* Time of day

## Visual Insights

### Geographic Analysis

* Accident distribution across regions
* Hotspot identification using maps

### Severity Analysis

* Comparison of fatal, serious, and slight accidents

### Demographic Analysis

* Driver age distribution
* Gender-based accident trends

### Vehicle Analysis

* Accident frequency by vehicle type
* Propulsion category comparisons

### Temporal Analysis

* Peak accident periods
* Time-of-day trends

### Environmental Analysis

* Impact of road conditions and junction controls

---

# Data Cleaning & Preparation

The following preprocessing steps are recommended or implemented:

1. Handling missing or null values.
2. Standardizing categorical variables.
3. Formatting date fields.
4. Verifying geographic coordinates.
5. Removing duplicate records.
6. Creating calculated measures in Power BI.
7. Building relationships and hierarchies for analysis.

---

# Suggested Data Model

A star-schema structure is recommended for scalability and performance:

## Fact Table

* Accident Facts

## Dimension Tables

* Date Dimension
* Location Dimension
* Vehicle Dimension
* Driver Dimension
* Road Condition Dimension

---

# Example Business Questions

This dashboard can help answer questions such as:

* Which UK regions experience the highest accident rates?
* What factors contribute most to severe accidents?
* Which vehicle types are most commonly involved in accidents?
* Are accidents more frequent in urban or rural areas?
* Which time periods show the highest accident occurrences?
* How do road conditions influence casualty rates?
* What demographic groups are most frequently involved in accidents?
* What is the estimated financial impact of accidents?

---

# Power BI Recommendations

## Recommended Visuals

* KPI Cards
* Line Charts
* Bar Charts
* Stacked Column Charts
* Filled Maps
* Heat Maps
* Matrix Tables
* Slicers

## Recommended DAX Measures

Examples:

```DAX
Total Accidents = SUM('Accidents'[Number of Accidents])

Total Casualties = SUM('Accidents'[Number of Casualties])

Total Accident Cost = SUM('Accidents'[Accidental Costs])

Average Casualties per Accident =
DIVIDE(
    [Total Casualties],
    [Total Accidents]
)
```

---

# Folder Structure

```text
project-folder/
│
├── UK Accident Information (Data Import).xlsx
│
├── Accident Report.pbix
│
├── dashboard-preview.png
│
└── README.md
```

---

# Expected Insights

The analysis is expected to reveal:

* High-risk accident regions
* Major contributing environmental factors
* Accident severity trends
* Demographic risk groups
* Vehicle involvement patterns
* Financial impact estimates
* Opportunities for road safety improvements

---

# Potential Improvements

Future enhancements may include:

* Integration with live government accident data
* Predictive accident modeling using machine learning
* Real-time dashboard updates
* Advanced geospatial analysis
* Weather API integration
* Traffic volume correlation analysis

---

# Conclusion

This project demonstrates how data analytics and interactive business intelligence tools can be used to better understand road accidents in the UK. Through effective visualization and exploration, the dashboard supports deeper insights into accident patterns, risk factors, and road safety trends.

The project can be extended for policy-making, transportation planning, insurance analysis, and public safety initiatives.

---

# Author

**Project:** UK Road Accident Analysis Dashboard
**Tool:** Microsoft Power BI
**Dataset:** UK Road Accident Information
