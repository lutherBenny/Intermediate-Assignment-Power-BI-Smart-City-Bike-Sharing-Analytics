# Smart City Bike Sharing Analytics Dashboard

## Dashboard Preview

### Dashboard 1 – Executive Overview
![Executive Overview](Screenshots/Executive-Overview.png)

### Dashboard 2 – City Performance & Station Analysis
![City Performance & Station Analysis](Screenshots/City-Performance-Station-Analysis.png)

---

## 1. Project Overview

The **Smart City Bike Sharing Analytics Dashboard** is an interactive Power BI project developed to analyse bike-sharing station data across different cities.

The dashboard provides insights into station availability, bike capacity, station status, banking facilities, bonus facilities, and city-wise performance.

## 2. Project Objectives

- Analyse the total number of bike-sharing stations.
- Monitor open and closed station status.
- Understand total bike capacity and available bikes.
- Compare bike capacity across cities.
- Analyse banking and bonus facility availability.
- Visualise station locations using a map.
- Present key insights through interactive Power BI dashboards.

## 3. Tools & Technologies

- **Microsoft Excel** – Dataset review and preparation
- **Power BI Desktop** – Dashboard development and data visualisation
- **Power Query** – Data cleaning and transformation
- **DAX** – Measures and calculated columns

## 4. Dashboard Details

### Page 1 – Executive Overview

Provides a high-level summary of the bike-sharing network.

**Key Performance Indicators (KPIs):**
- Total Bike Capacity
- Total Bike Stations
- Total Available Bikes
- Open Stations

**Visualisations:**
- Station Status Distribution – Donut Chart
- Bike Capacity by City – Bar Chart
- Available Bikes by City – Column Chart
- Banking Availability Distribution – Pie Chart

**Interactive Filters:**
- City / Contract Name
- Station Status
- Banking Availability

### Page 2 – City Performance & Station Analysis

Provides a detailed view of city-wise bike capacity, station locations, and facility availability.

**Visualisations:**
- Bonus Facility Distribution – Pie Chart
- Station Locations – Map
- Bike Availability – Gauge Chart
- Bike Capacity by City – Treemap

## 5. Dataset Information

The project uses a bike-sharing station dataset containing **2,856 records** and information about station locations, capacity, availability, and facilities.

**Important columns include:**
- Station Number
- Station Name
- Address
- Latitude
- Longitude
- Banking
- Bonus
- Status
- Contract Name
- Bike Stands
- Available Bike Stands
- Available Bikes
- Last Update

## 6. Data Cleaning & Transformation

Data preparation was performed using Power Query.

Key activities:
- Imported the original dataset into Power BI.
- Created separate Raw and Clean queries.
- Reviewed column quality, distribution, and data profiles.
- Split the Position column into Latitude and Longitude.
- Corrected column data types.
- Reviewed missing values, errors, and duplicate records.
- Created a validation check for bike capacity and availability.
- Created Banking Label and Bonus Label columns for clearer reporting.

## 7. DAX Measures

The following DAX measures were created for dashboard calculations:

```dax
Total Bike Stations =
COUNTROWS(Bike_Stations_Clean)

Total Bike Capacity =
SUM(Bike_Stations_Clean[Bike Stands])

Average Bike Capacity =
AVERAGE(Bike_Stations_Clean[Bike Stands])

Total Available Bikes =
SUM(Bike_Stations_Clean[Available Bikes])

Total Available Bike Stands =
SUM(Bike_Stations_Clean[Available Bike Stands])
```

## 8. Key Insights

Based on the dataset:

- **2,856** bike-sharing station records were analysed.
- **2,650** stations were marked as OPEN.
- **206** stations were marked as CLOSED.
- Approximately **57K** total bike capacity was recorded.
- Approximately **20K** available bikes were recorded.
- Banking facilities were available at approximately **11.76%** of stations.
- Bonus facilities were available at approximately **2.45%** of stations.

## 9. Project Scope & Data Limitations

This project focuses on bike-sharing station information and availability.

The dataset does not contain actual rental transactions, customer details, trip history, travel distance, or revenue information. Therefore, the dashboard does not analyse rental revenue or customer travel trends.

The Last Update column represents station update timestamps and should not be treated as a complete rental history.

## 10. Project Outcome

Successfully developed a two-page interactive Power BI dashboard using Power Query, DAX, charts, slicers, a map, a gauge, and a treemap.

This project helped strengthen practical skills in data cleaning, data modelling, DAX calculations, data visualisation, and dashboard development.



**Skills:** Excel | SQL | Power BI | Python | Data Analytics
