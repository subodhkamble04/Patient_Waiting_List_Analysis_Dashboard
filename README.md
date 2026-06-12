# Patient Waiting List Analysis Dashboard

## Project Overview

This project is an interactive Healthcare Analytics Dashboard developed using Microsoft Power BI. The dashboard helps analyze and monitor patient waiting lists across inpatient and outpatient categories between 2018 and 2021.

The project focuses on identifying waiting list trends, specialty-level analysis, age profile insights, and overall healthcare performance monitoring.

---

## Problem Statement

Healthcare organizations often face challenges in tracking and managing patient waiting lists efficiently. The objective of this project is to:

* Track the current status of patient waiting lists
* Analyze historical monthly trends of inpatient and outpatient waiting lists
* Perform specialty-level and age-profile analysis
* Provide interactive visual insights for better decision-making

---

## Objectives

* Monitor current waiting list statistics
* Compare Average vs Median waiting lists
* Analyze yearly and monthly patient trends
* Identify high waiting list specialties
* Enable granular analysis using interactive filters

---

## Dataset Information

### Data Scope

* Time Period: 2018 – 2021

### Data Sources

* Inpatient Data
* Outpatient Data
* Specialty Mapping Data

### Tools Used

* Microsoft Power BI
* Power Query
* DAX
* Excel/CSV Files

---

## Data Transformation Steps

The following preprocessing steps were performed using Power Query:

* Renamed inconsistent columns
* Rearranged column structures
* Added custom columns
* Appended inpatient and outpatient tables
* Removed trailing spaces
* Standardized inconsistent values
* Created relationships using data modeling

---

## DAX Measures Used

Some important DAX measures used in the dashboard:

```DAX
Latest Month Wait List =
CALCULATE(
    SUM(All_Data[Total]),
    All_Data[Archive_Date] = MAX(All_Data[Archive_Date])
) + 0
```

```DAX
Median Wait List =
MEDIAN(All_Data[Total])
```

```DAX
Average Wait List =
AVERAGE(All_Data[Total])
```

---

## Dashboard Features

### Summary Page

* KPI Cards
* Doughnut Charts
* Clustered Column Charts
* Trend Analysis
* Dynamic Average/Median Toggle
* Interactive Slicers

### Detailed View

* Matrix-based granular analysis
* Specialty-wise insights
* Age profile analysis
* Case type filtering

### Tooltip Page

* Interactive tooltip visualizations
* Specialty-level waitlist insights

---

## Key Insights

* Identified specialties with highest patient waiting times
* Compared inpatient and outpatient waiting list patterns
* Analyzed long-term healthcare demand trends
* Enabled dynamic filtering for deeper analysis

---

## Dashboard Screenshots

(Add your dashboard screenshots here)

---

## Learning Outcomes

Through this project, I gained practical experience in:

* Data Cleaning & Transformation
* Power Query Operations
* DAX Calculations
* Data Modeling
* Dashboard Design
* Interactive Data Visualization

---
