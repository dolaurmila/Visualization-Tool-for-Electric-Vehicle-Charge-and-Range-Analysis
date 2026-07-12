# Visualization Tool for Electric Vehicle Charge and Range Analysis

A Tableau-based analytics dashboard that brings together EV charging station data, vehicle/battery specifications, and pricing information into a single, role-based visualization tool for city energy planners, EV fleet managers, and prospective EV buyers.

🔗 **Tableau Public:** https://public.tableau.com/app/profile/urmila.dola/vizzes

🎥 **Demo Video:** https://drive.google.com/file/d/1RJBYEnAwOi4nLi9QWnntse60BQjl3vhk/view?usp=sharing

---

## Data Sources

- `EVIndia`
- `Electric_Car_DataClean`
- `ElectricVehicle_Charge_List`
- `Cheap_Electric_Cars_Vehicle`

**Scale:** 48 fields, 492 rows

## Data Preprocessing

1. **Data Collection** — Imported EV charging, vehicle, and battery datasets into MySQL and connected to Tableau.
2. **Data Cleaning** — Removed duplicate records and handled missing (NULL) values.
3. **Column Split** — Split the `CheapElectricCars` column into three columns.
4. **Rename** — Renamed the split-3 column to `Brands`.
5. **Data Type Change** — Changed the `Address` field to Geographic Role for map visualizations.
6. **Data Type Validation** — Verified data types across text, numeric, and categorical fields.
7. **Feature Selection** — Selected relevant fields: Brand, Vehicle Name, Price, Battery Capacity, Range, Charging Type, Region, Address.
8. **Calculated Fields** — Created `BodyStyle_Count` and `Car_Brands_India` for aggregated analysis.
9. **Data Extraction** — Converted the MySQL live connection to a Tableau Extract for performance and Tableau Public publishing.
10. **Data Validation** — Verified row counts, field values, and visualizations before building dashboards.

## Filters Used

Brand Name, Price, Region, Vehicle Name

## Calculated Fields

`BodyStyle_Count`, `Car_Brands_India`

## Visualizations

1. Brands According to Bodystyle
2. Brand Filtered by Powertrain Type
3. Top Brands in India (by efficiency)
4. Price for Different Cars in India
5. Top Speed for Different Brands
6. Different EV Cars in India
7. Charging Stations by Region and Type in India
8. Story of Electric Cars in India (charging stations, pricing, and brand comparisons)

## Dashboards

- **Dashboard 1** — EV Cars Globally & Brand Overview (India)
- **Dashboard 2** — Price, Brand Efficiency & Charging Stations Map

## Tech Stack

- **Data Storage:** MySQL
- **Visualization:** Tableau Desktop / Tableau Public
- **Data Prep:** Tableau Split, Calculated Fields, Data Type conversion

## Project Structure (Deliverables)

```
├── Ideation Phase
│   ├── Empathy Map Canvas
│   ├── Define Problem Statements
│   └── Brainstorming & Idea Prioritization
├── Requirement Analysis
│   ├── Customer Journey Map
│   ├── Solution Requirements (Functional & Non-functional)
│   ├── Data Flow Diagrams & User Stories
│   └── Technology Stack
├── Project Design
│   ├── Problem–Solution Fit Canvas
│   ├── Proposed Solution Template
│   └── Solution Architecture
├── Project Planning
│   └── Product Backlog, Sprint Schedule & Tracker
├── Testing
│   └── Project Performance Test
└── Results
    ├── Visualizations
    ├── Dashboards
    └── Story
```

## How to View

1. Open the workbook (`.twb`) in Tableau Desktop, **or**
2. Visit the published version on Tableau Public: https://public.tableau.com/app/profile/urmila.dola/vizzes
