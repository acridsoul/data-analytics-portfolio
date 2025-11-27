# Titanic Exploratory Data Analysis

**Student**: Austin Githinji
**Student ID**: CS-EH03-25417
**Program**: Cyber Shujaa - Data and Artificial Intelligence

## Overview

This project performs Exploratory Data Analysis (EDA) on the Titanic dataset to uncover patterns and relationships between passenger attributes and survival outcomes. The goal is to explore, clean, and analyze the data to identify factors that influenced survival.

## Dataset

- **Source**: [Titanic Dataset on Kaggle](https://www.kaggle.com/c/titanic)
- **Original Size**: 891 rows × 12 columns
- **Content**: Passenger data including PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, and Embarked

## Objectives

- Load and explore the Titanic dataset using pandas and seaborn
- Handle missing values, duplicates, and outliers to clean the data
- Perform univariate, bivariate, and multivariate analysis
- Visualize relationships among key variables (Age, Fare, Sex, Pclass, Survived)
- Analyze the target variable (Survived) and determine factors influencing survival
- Present findings with supporting visualizations

## Tasks Completed

### 1. Initial Data Exploration
- Loaded dataset and displayed first 5 rows
- Checked dataset shape, column names, and data types
- Generated descriptive statistics for numerical and categorical columns
- Identified missing values: Cabin (77.1%), Age (19.9%), Embarked (0.2%)

### 2. Data Cleaning
- Dropped Cabin column (too many missing values)
- Filled missing Age values with median
- Filled missing Embarked values with mode (most frequent)
- Verified all missing values handled

### 3. Outlier Detection and Treatment
- Created boxplots to visualize outliers in Age and Fare
- Applied IQR (Interquartile Range) method to detect outliers in Fare
- Capped outliers at upper and lower bounds

### 4. Univariate Analysis
- Analyzed categorical features: Sex, Pclass, Embarked
- Created count plots for gender, passenger class, and embarkation distribution
- Generated histograms with KDE for Age and Fare distributions
- Calculated descriptive statistics for numerical features

### 5. Bivariate Analysis
- Created correlation heatmap for numerical features
- Analyzed survival rates by:
  - Passenger Class
  - Gender
  - Embarkation Port
- Visualized Age and Fare distributions by survival status using boxplots

### 6. Multivariate Analysis
- Examined combined effects of Class and Gender on survival
- Created scatter plots showing Age, Fare, Survival, and Class relationships
- Generated crosstab heatmap for Embarkation Port, Class, and Survival
- Analyzed interaction effects between Gender, Class, and Embarkation

### 7. Target Variable Analysis
- Visualized survival distribution (38.38% overall survival rate)
- Analyzed survival by Gender and Class combinations
- Examined survival by Embarkation and Gender

### 8. Validation and Export
- Verified no missing values after cleaning
- Confirmed correct data types
- Checked for duplicate rows (none found)
- Validated data ranges for Age and Fare
- Exported cleaned dataset as `cleaned_titanic.csv`

## Key Findings

- **Overall Survival Rate**: 38.38%
- **Gender Impact**: Females had significantly higher survival rates than males
- **Class Impact**: First-class passengers had higher survival rates than lower classes
- **Combined Effect**: First-class females had the highest survival rate
- **Embarkation**: Port of embarkation showed some correlation with survival
- **Social Factors**: Gender and class were crucial factors determining survival chances

## Files

- `titanic-eda.ipynb` - Complete EDA notebook with 24 cells
- `cleaned_titanic.csv` - Cleaned dataset (891 rows)
- `Austin_Githinji_CS_EH03_25417.pdf` - Assignment report

## Technologies Used

- Python 3
- pandas
- numpy
- matplotlib
- seaborn

## Visualizations Created

- Boxplots for outlier detection
- Count plots for categorical distributions
- Histograms with KDE for numerical features
- Correlation heatmap
- Bar plots for survival rates by categories
- Scatter plots for multivariate relationships
- Crosstab heatmaps

## Conclusion

This EDA successfully demonstrated the data wrangling and analytical process applied to the Titanic dataset. Through structured analysis, key patterns affecting survival were identified. The dataset is now clean, validated, and ready for predictive modeling or deeper statistical inference.

Social and economic factors (gender and class) played a crucial role in survival chances during the Titanic disaster.

## Kaggle Notebook

View the interactive notebook: [https://www.kaggle.com/code/austingithinji/austin-githinji-t-cs-eh03-25417](https://www.kaggle.com/code/austingithinji/austin-githinji-t-cs-eh03-25417)
