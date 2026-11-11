# Ride-Hailing Trip Analytics Platform

## Project Overview
An end-to-end ride-hailing analytics project built using Databricks and Medallion Architecture.

The project transforms raw ride data into clean, analytics-ready data and presents business insights through an interactive dashboard.

## Technologies Used
- Databricks
- SQL
- Python and PySpark
- Lakeflow Spark Declarative Pipelines
- Databricks AI/BI Dashboards
- Medallion Architecture

## Data Architecture

### Bronze Layer
Stores raw ride trip data.

Table: `ride_trips_bronze`

### Silver Layer
Cleans data, removes duplicate trip IDs, and separates invalid records.

Tables:
- `ride_trips_silver`
- `ride_trips_rejected`

### Gold Layer
Contains business summary tables.

- `gold_monthly_trips`
- `gold_city_summary`
- `gold_vehicle_summary`
- `gold_payment_summary`
- `gold_rating_summary`
- `gold_data_quality`

## Data Quality Results

| Category | Records |
|---|---:|
| Bronze | 1,214 |
| Clean Silver | 1,168 |
| Rejected | 22 |
| Duplicates | 24 |

**Reconciliation:**

1,214 = 1,168 + 22 + 24

**Status: PASS**

## Dashboard Pages

1. Executive Overview
2. Vehicle & Payment Analysis
3. Data Quality & Reconciliation

## Business Metrics
- Total Trips
- Net Revenue
- Total Distance
- Platform Earnings
- Average Customer Rating
- Pending Payment Amount

## Screenshots

Project screenshots are included in this repository.

## Project Outcome

Successfully implemented an end-to-end ride-hailing analytics platform using Databricks, including data cleaning, validation, business analytics, reconciliation, and an interactive published dashboard.
