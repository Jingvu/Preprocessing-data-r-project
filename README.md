# Preprocessing Data
In this project, I applied my data wrangling and preprocessing skills to the Anime Dataset 2023 from Kaggle with the goal of cleaning, transforming, and preparing it for analysis. The dataset included user ratings, anime metadata, and user demographics, and I focused on ensuring data quality and consistency throughout. Key tasks involved importing and merging data, handling missing values, handling outliers, transforming variables, and visualizing results to extract meaningful insights. I particularly concentrated on three crucial areas: transforming data for better distribution, handling outliers to avoid skewed analysis, and managing missing values using various techniques. This repository not only demonstrates my approach to solving these challenges but also serves as a helpful resource with R code examples for anyone interested, as well as a reference for my future projects.

## Key Features of the Project
### 1. Data Import & Merging:
- Importing datasets from CSV and Excel files using R libraries (readxl, readr).
- Merging two datasets (anime ratings and user details) to create a comprehensive dataset using left_join.

### 2. Data Cleaning & Preprocessing:
- Data type conversions: Converted columns like dates and categorical variables to their appropriate data types.
- Data tidying: Cleaned up columns with untidy and non-standard entries
  + The genre column contained multiple values separated by commas, listing all genres within a single cell.
  + The location column, which combined both city and country information and has non-standard country names.
- Handling missing values: Used various techniques:
  + Imputing missing values for numerical columns with the median.
  + Filling categorical columns with meaningful defaults.
  + Applying predictive modeling (mice package) for missing date values.
- Detecting & handling special value (infinite, NaN).
- Identifying potential data entry errors.

### 3. Handling Outliers:
- Detecting outliers
- Handling outliers using capping techniques to preserve data integrity while minimizing the impact of extreme values.

### 4. Data Transformation:
- Applied various mathematical transformations (square, cube, Box-Cox, log, log10, square root, cube root, reciprocal and reciprocal square) to make their distributions closer to normal, improving the accuracy of subsequent analyses.

## The Principle
### 1. Missing Value Imputation
