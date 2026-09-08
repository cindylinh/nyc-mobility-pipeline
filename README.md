# NYC Mobility Pipeline & Insights

**Taxi Zone Prioritisation for Targeted Mobility Interventions**

An end-to-end data engineering and analytics project that analyses NYC taxi, subway, bus and Citi Bike data to identify taxi zones that may warrant further mobility service-planning review.

## Project Overview

This project built a reproducible data pipeline using over **16.8 million mobility records** across NYC taxi, subway, bus and Citi Bike datasets.

The analysis focused on identifying taxi zones with different mobility demand patterns based on:

- Taxi demand volume
- Time-of-day demand
- Short- and long-trip patterns
- Comparison with subway, bus and Citi Bike activity

The pipeline included data sourcing, auditing, cleaning, transformation, SQL analysis and intervention-priority classification.

## Key Findings

- **Manhattan accounted for 3.2M of 3.7M taxi trips**, showing a strong concentration of taxi demand
- **58.6% of Manhattan trips were under 2 miles**, indicating potential areas for short-trip alternative transport review
- **Queens had the strongest long-trip pattern at 79.3%**, largely influenced by JFK and LaGuardia airport travel
- Taxi demand peaked during the **evening period (17:00–21:00)**
- **73 taxi zones** were identified for further review across four intervention categories:
  - 29 zones — Taxi pickup/drop-off management
  - 27 zones — Late-night public transport support
  - 7 zones — Short-trip alternative transport review
  - 10 zones — Public transport connectivity review

## Data Pipeline & Methods

- **Data sourcing:** Direct public dataset downloads and Socrata API pagination
- **Data processing:** Python, pandas and DuckDB
- **Data auditing:** Percentage-based severity classification across six datasets
- **Data cleaning:** Standardisation, missing-value assessment and data-quality checks
- **Feature engineering:** Time-period classification, trip-distance features and geographic enrichment
- **SQL analysis:** Multi-stage analysis across 16 engineered DuckDB tables
- **Geographic analysis:** NYC taxi zone lookup and GeoPandas
- **Data governance:** Privacy-aware aggregation and responsible interpretation of mobility data

## Tools and Techniques

- Python
- SQL
- DuckDB
- pandas
- GeoPandas
- Google Colab
- Socrata API
- Data Cleaning & Transformation
- Data Auditing
- Feature Engineering
- Exploratory Data Analysis
- Data Visualisation

## Project Files

- [View full analysis notebook](NYC_Mobility_Pipeline.ipynb)
- [View full project report](NYC_Mobility_Pipeline_and_Insights.pdf)

## Data Sources

- NYC TLC Yellow Taxi Trip Records
- NYC TLC Green Taxi Trip Records
- MTA Subway Hourly Ridership
- MTA Bus Hourly Ridership
- Citi Bike Trip Data
- NYC Taxi Zone Lookup

---

*This project used publicly available, aggregated mobility data. No individual identities, passenger information, or individual trip paths were analysed or visualised.*
