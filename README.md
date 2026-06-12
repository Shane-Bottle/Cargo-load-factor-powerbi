# Cargo Load Factor Dashboard | Power BI

## Overview
An interactive Power BI dashboard analysing cargo load factor performance 
across Emirates-style routes, aircraft types, and monthly trends.

Built as part of a self-directed data analytics portfolio by a Senior Airport 
Service Agent transitioning into data analytics — combining 12+ years of 
aviation operations experience with self-taught BI skills.

---

## Dashboard Features
- **KPI Cards** — Total Flights, Avg Load Factor %, Total Revenue USD, Total Weight Loaded kg
- **Bar Chart** — Avg Load Factor % by Route (DXB network)
- **Line Chart** — Monthly Load Factor % trend (Jan–Dec 2024)
- **Column Chart** — Total Revenue by Aircraft Type
- **Slicers** — Filter by Aircraft Type and Route

---

## DAX Measures Used
```DAX
Total Flights = COUNTROWS(cargo_load_factor)

Avg Load Factor % = AVERAGE(cargo_load_factor[LoadFactor_pct])

Total Revenue USD = SUM(cargo_load_factor[Revenue_USD])

Total Weight Loaded kg = SUM(cargo_load_factor[ActualLoad_kg])
```

---

## Dataset
- 600 rows of simulated cargo flight data
- Routes: DXB → LHR, JFK, ORD, SIN, SYD, HKG, NRT, FRA, CDG, BOM, DEL, CGO
- Aircraft: B777F, B747-8F, B777-200LRF
- Period: January 2024 – December 2024

---

## Tools Used
- Power BI Desktop
- DAX
- Power Query

---

## Key Insights
- DXB → BOM and DXB → CDG recorded highest avg load factor (77%)
- DXB → LHR recorded lowest avg load factor (72%)
- B747-8F generated highest total revenue ($64M)
- Load factor peaked in March and September, dipped in May and December

---

## Author
**Shane Dodwell Holdenbottle**  
Senior Airport Service Agent | Emirates Airlines  
Self-directed Data Analytics Portfolio  
Dubai, U.A.E
