# Telco Customer Churn Analysis

## Project Overview

This project focuses on exploring and understanding customer churn in the telecommunications industry using Python. The analysis investigates customer behaviour, service usage, subscription patterns and the factors associated with customer churn.

The main objective is to identify meaningful patterns in the dataset through data cleaning, exploratory data analysis (EDA) and data visualization.

## Dataset

The dataset contains **7,043 customer records and 21 original features**, covering customer demographics, subscribed services, account information and churn status.

**Dataset:** Telco Customer Churn Dataset

## Tools & Technologies

- Python
- Pandas – Data manipulation and cleaning
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Jupyter Notebook – Data analysis environment

## Project Workflow

### 1. Data Understanding
- Inspected the dataset structure and dimensions.
- Reviewed column data types.
- Examined descriptive statistics.
- Identified categorical and numerical variables.

### 2. Data Cleaning
- Checked for duplicate records and duplicate customer IDs.
- Handled whitespace and inconsistent text values.
- Converted `TotalCharges` into a numerical data type.
- Identified 11 blank `TotalCharges` values.
- Replaced these values with 0 because the corresponding customers had zero tenure.
- Created an indicator to preserve the original missing-value information.
- Verified missing values and duplicate records after cleaning.

### 3. Feature Engineering

The following additional features were created:

| Feature | Description |
|---|---|
| `tenure_group` | Groups customers according to their tenure |
| `total_services` | Counts the services subscribed to by each customer |
| `churn_flag` | Converts churn status into numerical values |
| `long_term_customer` | Identifies customers with 24 or more months of tenure |
| `total_charges_was_missing` | Preserves the original missing-value status of TotalCharges |

### 4. Exploratory Data Analysis

The analysis follows these sections:

- Univariate Analysis
- Bivariate Analysis
  - Numerical vs Numerical
  - Numerical vs Categorical
- Categorical Relationship Analysis
- Correlation Analysis
- Outlier Analysis
- Summary of Findings

## Key Findings

- The overall customer churn rate is approximately **26.54%**.
- Month-to-month contract customers have a higher churn rate than customers with longer-term contracts.
- Customers with shorter tenure show higher churn rates.
- Customers with longer subscription periods generally demonstrate lower churn rates.

These findings represent descriptive associations within the dataset and do not establish causation.

## Final Dataset

After cleaning and feature engineering, the final dataset contains:

- **7,043 records**
- **26 columns**
- **0 missing values**
- **0 duplicate rows**
- **0 duplicate customer IDs**

## Project Objective

This project demonstrates practical skills in data cleaning, feature engineering, exploratory data analysis and data visualization. It also explores how analytical techniques can be used to identify customer churn patterns and generate meaningful business insights.

---

**Project Category:** Data Analytics / Exploratory Data Analysis  
