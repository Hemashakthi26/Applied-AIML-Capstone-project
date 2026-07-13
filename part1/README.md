# Applied AI & ML Essentials - Capstone Project (Part 1)

## Project Title
Data Acquisition, Cleaning and Exploratory Data Analysis (EDA) on Stroke Prediction Dataset

## Dataset Description

This project uses the Stroke Prediction Dataset obtained from Kaggle. The dataset contains patient health and demographic information used to analyze factors associated with stroke occurrence.

### Dataset Information
- Number of Rows: 5110
- Number of Columns: 12

Features include:
- Gender
- Age
- Hypertension
- Heart Disease
- Ever Married
- Work Type
- Residence Type
- Average Glucose Level
- BMI
- Smoking Status
- Stroke (Target Variable)

## Objective

The objective of this project is to clean the raw dataset, handle missing values, analyze data quality, identify outliers, perform exploratory data analysis (EDA), and prepare a cleaned dataset for machine learning in Part 2.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn

## Tasks Performed

### 1. Data Loading
- Loaded the dataset using pandas.read_csv().
- Displayed the first five rows.
- Checked dataset shape and data types.

### 2. Missing Value Analysis
- Calculated missing values and their percentages.
- BMI contained approximately 3.93% missing values.
- Missing BMI values were filled using the median.

### 3. Duplicate Detection
- Checked for duplicate rows.
- Removed duplicates if present.

### 4. Data Type Conversion
- Converted repetitive string columns to the category data type.
- Compared memory usage before and after conversion.

### 5. Descriptive Statistics
- Generated summary statistics using describe().

### 6. Skewness Analysis
- Calculated skewness for continuous numerical columns.
- avg_glucose_level showed the highest positive skewness (1.57).
- Since the data is positively skewed, the median was preferred over the mean for imputation because the mean is influenced by extreme values.

### 7. Outlier Detection
Used the IQR method on:
- Average Glucose Level
- BMI

Outliers were documented but not removed because they may represent genuine medical observations.

### 8. Visualizations
The following visualizations were created:
- Line Plot
- Bar Chart
- Histogram
- Scatter Plot
- Box Plot
- Correlation Heatmap

### 9. Correlation Analysis
- Computed the Pearson Correlation Matrix.
- Computed the Spearman Correlation Matrix.
- Compared Pearson and Spearman correlations.

### 10. Grouped Aggregation
Performed grouped statistical analysis using:
- Mean
- Standard Deviation
- Count

for BMI across different Work Types.

### 11. Clean Dataset
The cleaned dataset was saved as:
cleaned_data.csv

## Key Findings

- BMI contained a small number of missing values.
- Median imputation was selected because it is more robust to skewed distributions.
- Average Glucose Level was the most positively skewed continuous feature.
- Outliers were identified using the IQR method but retained for future modeling.
- Correlation analysis was performed to understand relationships among numerical variables.

## Project Structure

part1/
├── data/
├── plots/
├── cleaned_data.csv
├── part1_data_cleaning_EDA.ipynb
└── README.md

## Author

Hemashakthi M

Applied AI & ML Essentials Capstone Project
