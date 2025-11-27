# Netflix Data Wrangling Project

**Student**: Austin Githinji
**Student ID**: CS-EH03-25417
**Program**: Cyber Shujaa - Data and Artificial Intelligence

## Overview

This project demonstrates hands-on data wrangling skills using the Netflix Movies and TV Shows dataset from Kaggle. The goal was to clean, structure, and transform raw data into a format suitable for analysis.

## Dataset

- **Source**: [Netflix Shows Dataset by Shivam Bansal](https://www.kaggle.com/shivamb/netflix-shows)
- **Original Size**: 8,807 rows × 12 columns
- **Content**: Metadata about Netflix titles including type, director, cast, country, release year, duration, and genres

## Tasks Completed

### 1. Loading and Exploring
- Loaded dataset using pandas
- Checked structure, shape, and data types
- Identified missing values and duplicates

### 2. Data Discovery
- Examined data types for each column
- Found missing values: 2,634 directors, 825 cast members, 831 countries
- Confirmed no duplicate rows

### 3. Structuring
- Converted `date_added` to datetime format
- Split `duration` column into `duration_value` (numeric) and `duration_unit` (text)

### 4. Cleaning
- Removed duplicate rows
- Dropped `description` column (not needed)
- Filled missing values with "Not Given" for director, cast, and country
- Dropped rows with critical nulls in date_added, rating, and duration

### 5. Transformation and Enrichment
- Filtered dataset to get Movies only
- Sorted titles by most recent release year
- Grouped by country to count titles per country
- **Top Country**: United States with 2,775 titles

### 6. Validation
- Checked for logical inconsistencies (14 titles where date_added < release_year)
- Verified data types after cleaning
- Sampled random rows for manual inspection
- Reset index for clean output

### 7. Export
- Saved cleaned dataset as `cleaned_netflix.csv`
- Final dataset: 8,810 rows × 13 columns

## Files

- `netflix-data-wrangling.ipynb` - Main notebook with complete workflow
- `cleaned_netflix.csv` - Cleaned and processed dataset
- `Austin_Githinji_cs-eh03-25417.pdf` - Assignment report

## Key Findings

- United States has the most titles (2,775)
- India comes second with 971 titles
- 826 titles have no country information
- 14 records show inconsistent dates (added before release year)

## Technologies Used

- Python 3
- pandas
- datetime

## Kaggle Notebook

View the interactive notebook: [https://www.kaggle.com/code/austingithinji/austin-githinji-cs-eh03-25417](https://www.kaggle.com/code/austingithinji/austin-githinji-cs-eh03-25417)
