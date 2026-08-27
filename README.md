# Elevate Labs - Task 1: Data Cleaning and Preprocessing

## Objective

The objective of this task was to clean and preprocess a raw dataset using Python and Pandas. The goal was to identify and handle common data-quality issues and prepare the dataset for further analysis or modelling.

## Dataset

Dataset: Customer Personality Analysis

The dataset contains customer demographic information, purchasing behavior, product spending, and marketing campaign response data.

- Rows: 2,240
- Columns: 29
- Tool: Python (Pandas)
- Environment: Jupyter Notebook

## Data Cleaning and Preprocessing

The following cleaning and preprocessing steps were performed:

1. Inspected the dataset structure, rows, columns, and data types.
2. Identified missing values using Pandas.
3. Filled missing values in the Income column using the median income.
4. Checked for duplicate records; no duplicates were found.
5. Identified unrealistic birth years and treated them as missing values.
6. Identified the anomalous Income value 666666 and replaced it with the median income.
7. Standardized inconsistent Marital_Status values such as Alone, Absurd, and YOLO into Other.
8. Converted Dt_Customer from text to a proper datetime format.
9. Standardized column names to lowercase with underscores.
10. Performed final data-quality checks after cleaning.

## Repository Structure

ElevateLabs_Task1_Customer_Personality_Analysis/
│
├── Data/
│   ├── customer_personality_raw.csv
│   └── customer_personality_cleaned.csv
│
├── Notebook/
│   └── Task1_Data_Cleaning.ipynb
│
└── README.md

## Files

- customer_personality_raw.csv - Original raw dataset.
- customer_personality_cleaned.csv - Cleaned and preprocessed dataset.
- Task1_Data_Cleaning.ipynb - Jupyter Notebook containing the complete cleaning process.
- README.md - Project documentation and summary of preprocessing steps.

## Final Result

The Customer Personality Analysis dataset was successfully cleaned and preprocessed.

Final dataset:
- 2,240 records
- 29 columns

The cleaned dataset is ready for further analysis or modelling.

## Key Learning

This task provided practical experience in:

- Handling missing values
- Detecting duplicate records
- Handling invalid and anomalous data
- Standardizing categorical values
- Converting dates to datetime
- Checking data types
- Standardizing column names
- Performing data-quality validation using Pandas

## Technologies Used

Python | Pandas | Jupyter Notebook

## Status

Completed

This task was completed as part of the Elevate Labs Data Analytics Internship.
