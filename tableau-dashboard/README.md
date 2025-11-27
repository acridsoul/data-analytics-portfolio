# HR Analytics Dashboard - Tableau

**Student**: Austin Githinji
**Student ID**: CS-EH03-25417
**Program**: Cyber Shujaa - Data and Artificial Intelligence

## Overview

This project demonstrates data visualization skills using Tableau to build an interactive HR Analytics Dashboard. The dashboard provides HR managers with both high-level KPIs and detailed employee data with filtering capabilities.

## Dataset

- **Source**: HumanResources-Kenyan.csv
- **Content**: Employee information including demographics, job roles, hire dates, salaries, and termination dates
- **Employees**: 7,950 total (1,000 active, 8,950 terminated)

## Objectives

- Apply data visualization principles using Tableau Public
- Load and transform raw CSV dataset within Tableau
- Create calculated measures to derive key business metrics
- Build multiple visualization types (KPI cards, bar charts, tables)
- Combine worksheets into a cohesive interactive dashboard
- Publish dashboard to Tableau Public for sharing

## Tasks Completed

### 1. Data Loading and Preparation
- Connected to CSV file and loaded employee data
- Renamed fields for clarity (e.g., employee_id ’ Employee Id)
- Created Job Roles hierarchy (Department ’ Job Title) for drill-down capability

### 2. Calculated Measures
Created three key metrics using formulas:
- **Total Employees**: Count of all employees (1)
- **Active Employees**: `IF ISNULL([Termdate]) THEN 1 ELSE 0 END`
- **Terminated Employees**: `IF NOT ISNULL([Termdate]) THEN 1 ELSE 0 END`

### 3. Visualization Worksheets

Built four separate worksheets:

**Overview KPIs**
- Text-based display of headcount metrics
- Shows Total, Active, and Terminated employee counts
- Provides at-a-glance summary

**Demographics Analysis**
- Bar chart showing employee count by Gender
- Visual breakdown of workforce composition

**Income Analysis**
- Bar chart displaying Average Salary by Department
- Changed aggregation from SUM to AVG
- Formatted labels as currency

**Employee List**
- Detailed table with employee information
- Columns: Employee ID, Name, Department, Job Title, Hire Date, Salary
- Interactive filters for Department and Job Title

### 4. Dashboard Assembly
- Created new dashboard with automatic sizing
- Arranged four worksheets in logical layout
- Enabled "Use as Filter" on Demographics and Income Analysis charts
- Clicking any bar filters the Employee List table dynamically

### 5. Advanced Features
- Implemented custom tooltips with trend line charts
- Added data bars to employee table for visual comparison
- Applied professional color scheme and formatting
- Published to Tableau Public cloud

## Key Metrics

- **Total Employees**: 7,950
- **Active Employees**: 1,000
- **Terminated Employees**: 8,950
- **Departments Analyzed**: Multiple (Engineering, Sales, HR, Finance, etc.)

## Features

- **Interactive Filtering**: Click on any demographic or department to filter employee list
- **Hierarchical Navigation**: Drill down from Department to Job Title
- **Dynamic Tooltips**: Hover over KPIs to see trend charts
- **Responsive Layout**: Automatic sizing for different screen sizes

## Files

- `Tableau Workbook.twbx` - Complete Tableau workbook with all visualizations
- `Austin_Githinji_CS_EH30_25417.pdf` - Assignment report with screenshots

## Tools Used

- Tableau Public
- Data transformation and calculated fields
- Interactive dashboards and filtering

## Skills Demonstrated

- Data connection and preparation
- Calculated field creation
- Multiple visualization types (KPIs, bar charts, tables)
- Dashboard design and layout
- Interactive filtering and drill-down
- Custom tooltips and formatting
- Publishing to Tableau Public

## Dashboard Link

[View Dashboard on Google Drive](https://drive.google.com/drive/folders/10Y5kRb5ivDMipJ5rnPObtKa_5Q0NK3zT?usp=drive_link)

## Conclusion

This project successfully demonstrates the end-to-end Tableau workflow from data loading to publishing an interactive dashboard. The final product transforms raw employee data into an insightful decision-making tool that meets HR management needs for both summary metrics and detailed analysis.
