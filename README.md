# Task 1 - Customer Personality Analysis: Data Cleaning & Preprocessing

## 📌 Objective

The objective of this task was to clean and preprocess a raw dataset using Python and Pandas.

The goal was to identify and fix common data-quality issues such as missing values, duplicate records, inconsistent values, incorrect data types, and formatting issues, making the dataset ready for further analysis.

## 📊 Dataset

**Dataset:** Customer Personality Analysis

The dataset contains customer demographic information, purchasing behavior, product spending, and marketing campaign response data.

- **Rows:** 2,240
- **Columns:** 29
- **Tool Used:** Python (Pandas)

## 🛠️ Tools & Technologies

- Python
- Pandas
- Jupyter Notebook

## 🧹 Data Cleaning & Preprocessing

The following data-cleaning steps were performed:

### 1. Dataset Inspection
- Checked the number of rows and columns.
- Inspected column names and data types.
- Reviewed the overall structure of the dataset.

### 2. Missing Values
- Identified missing values using `isnull()`.
- Found missing values in the `Income` column.
- Filled the missing income values using the median income.

### 3. Duplicate Records
- Checked for duplicate rows using `duplicated()`.
- No duplicate records were found in the dataset.

### 4. Invalid Birth Years
- Identified unrealistic birth years such as 1893, 1899, and 1900.
- Treated these invalid values as missing values for better data quality.

### 5. Income Anomaly
- Identified an unusual income value of `666666`.
- Treated it as an anomalous value and replaced it with the median income.

### 6. Standardizing Categorical Values
Inconsistent marital-status values were identified:

- `Alone`
- `Absurd`
- `YOLO`

These values were grouped under:

`Other`

### 7. Date Formatting
- Converted the `Dt_Customer` column from text to a proper datetime data type.
- Used a consistent day-first date interpretation.

### 8. Column Name Standardization
Column names were standardized into a clean and uniform format:

- Converted names to lowercase.
- Removed unnecessary spaces.
- Used underscores for readability.

For example:

`Year_Birth` → `year_birth`

`Marital_Status` → `marital_status`

`Dt_Customer` → `dt_customer`

### 9. Final Data Quality Check
After cleaning, the dataset was checked again for:
- Missing values
- Duplicate records
- Data types
- Overall dataset structure

## 📁 Repository Structure

```text
ElevateLabs_Task1_Customer_Personality_Analysis/
│
├── Data/
│   ├── customer_personality_raw.csv
│   └── customer_personality_cleaned.csv
│
├── Notebook/
│   └── Task1_Customer_Personality_Cleaning.ipynb
│
└── README.md
