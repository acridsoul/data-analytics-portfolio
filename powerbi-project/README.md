# Hospitality Revenue Dashboard - Power BI

**Student**: Austin Githinji
**Student ID**: CS-EH03-25417
**Program**: Cyber Shujaa - Data and Artificial Intelligence

## Overview

This project demonstrates end-to-end Business Intelligence skills using Power BI to build a comprehensive revenue analytics dashboard for AtliQ Grands, a fictional five-star hotel chain. The dashboard provides insights into booking patterns, revenue metrics, and occupancy rates to support strategic decision-making.

## Business Context

AtliQ Grands hotel chain needed a BI solution to analyze booking and revenue data across multiple properties. The dashboard helps management understand key performance indicators, identify revenue optimization opportunities, and analyze weekday vs. weekend patterns.

## Dataset

**Data Sources** (CSV files):
- `dim_date.csv` - Date dimension table
- `dim_hotels.csv` - Hotel properties information
- `dim_rooms.csv` - Room types and categories
- `fact_bookings.csv` - Detailed booking transactions (13 MB)
- `fact_aggregated_bookings.csv` - Aggregated booking summaries (245 KB)

## Objectives

- Understand business requirements for hotel revenue analytics
- Load and transform multiple data sources using Power Query
- Build relational data model using star schema
- Create calculated columns and measures using DAX
- Develop interactive dashboard for effective decision-making
- Publish report to Power BI service

## Tasks Completed

### 1. Data Loading and Transformation
- Connected to folder containing CSV files
- Loaded all tables into Power Query editor
- Promoted headers and verified data types
- Removed irrelevant columns
- Prepared data for modeling

### 2. Building the Data Model
- Created star schema architecture
- **Fact Tables**: fact_bookings, fact_aggregated_bookings (center)
- **Dimension Tables**: dim_date, dim_hotels, dim_rooms (surrounding)
- Established relationships using common keys (property_id, room_id, date)
- Organized tables in logical model view

### 3. Creating DAX Columns and Measures

**Calculated Columns**:
- `day_type` in dim_date table - classifies dates as "Weekday" or "Weekend" (Friday and Saturday = Weekend)

**Key Measures** (stored in "Key Measures" table):
- **Total Revenue** - Overall revenue calculation
- **ADR** (Average Daily Rate) - Average revenue per room sold
- **RevPAR** (Revenue Per Available Room) - Revenue efficiency metric
- **Occupancy %** - Room utilization percentage
- **Realization %** - Booking success rate

### 4. Visualizing the Dashboard

**Filters/Slicers**:
- City filter
- Room Class filter
- Month selector
- Week Number selector

**KPI Cards**:
- Revenue: 1.69bn
- Occupancy: 57.8%
- Average Rating: 3.62
- RevPAR and other key metrics

**Main Visuals**:
- Detailed table with metrics per hotel property
- Revenue by City
- Occupancy % by City
- Average Rating by City
- Weekday vs. Weekend analysis (Occupancy, RevPAR, ADR)
- Booking breakdown by platform
- Revenue trends over time

### 5. Advanced Features
- **Custom Tooltips**: Hover over KPI cards to see week-by-week trend charts split by Business and Luxury hotel types
- **Data Bars**: Added to tables for easy visual comparison
- **Professional Formatting**: Custom color scheme and styling
- **Interactive Filtering**: All visuals respond to slicer selections

## Key Metrics

- **Total Revenue**: 1.69 billion
- **Occupancy Rate**: 57.8%
- **Average Rating**: 3.62
- **Weekend Revenue**: 2 billion
- **Primary Booking Platform**: Direct bookings

## Key Insights

- Dashboard revealed the hotel chain's **lack of a dynamic pricing strategy**
- Weekday vs. weekend revenue patterns identified
- Occupancy variations across different cities and properties
- Booking platform preferences analyzed

## Features

- **Star Schema Data Model** - Optimized for performance and scalability
- **DAX Calculations** - Custom business metrics and KPIs
- **Interactive Slicers** - Drill down by city, room class, month, and week
- **Trend Analysis** - Week-by-week performance tracking
- **Multi-dimensional Analysis** - Compare metrics across properties, time periods, and room types

## Files

- `powerbi-file.pbix` - Complete Power BI project file (2.2 MB)
- `wk4files/` - Source data files (CSV)
- `05-DAX-metrics-list.xlsx` - DAX formulas documentation
- `Austin_Githinji_CS_EH30_25417.pdf` - Assignment report with screenshots

## Tools Used

- Power BI Desktop
- Power Query (data transformation)
- DAX (Data Analysis Expressions)
- Star schema data modeling

## Skills Demonstrated

- Business Intelligence development
- Power Query data transformation
- Star schema data modeling
- DAX formula creation
- Interactive dashboard design
- KPI visualization
- Custom tooltips and formatting
- Multi-table relationships

## Conclusion

This project successfully demonstrates the complete Power BI workflow from understanding business needs to creating an interactive dashboard. The solution provides meaningful insights into hotel performance and uncovers opportunities for revenue optimization through dynamic pricing strategies.

The dashboard serves as a powerful decision-making tool for hotel management, enabling data-driven strategies to improve occupancy rates and maximize revenue.
