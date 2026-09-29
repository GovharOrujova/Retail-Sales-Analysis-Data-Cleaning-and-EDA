# Retail-Sales-Analysis-Data-Cleaning-and-EDA
Exploratory data analysis of retail store sales using Python. This project examines sales performance, product categories, customer transactions, payment methods, locations, discounts, time-based trends, missing values, distributions, and correlations using Pandas, NumPy, Matplotlib, and Seaborn.

# Retail Sales Analysis

## Description

This project performs an exploratory data analysis (EDA) of retail store sales data using Python. The analysis focuses on data quality, sales performance, customer transactions, product categories, payment methods, locations, discounts, time-based trends, and relationships between numerical variables.

The project is implemented in a Jupyter Notebook using **Pandas, NumPy, Matplotlib, and Seaborn**.

## Dataset

The dataset contains **12,575 transactions** and **11 columns** covering transactions from **January 1, 2022 to January 18, 2025**.

### Main Columns

* `Transaction ID` — unique transaction identifier
* `Customer ID` — customer identifier
* `Category` — product category
* `Item` — item identifier
* `Price Per Unit` — unit price
* `Quantity` — quantity purchased
* `Total Spent` — total transaction amount
* `Payment Method` — payment method
* `Location` — Online or In-store
* `Transaction Date` — transaction date
* `Discount Applied` — discount information

## Analysis Performed

### 1. Data Understanding

* Previewed the first and last records
* Checked dataset shape and structure
* Inspected columns and data types
* Generated descriptive statistics

### 2. Data Quality

* Checked missing values and missing-value percentages
* Visualized missing values
* Checked duplicated records
* Reviewed unique values and category distributions

### 3. Feature Engineering

The `Transaction Date` column was converted to datetime and the following features were created:

* `Year`
* `Month`
* `Day`
* `Day of Week`
* `Month Name`

A `Calculated Total` column was also created using:

```text
Price Per Unit × Quantity
```

The calculated value was compared with `Total Spent`.

### 4. Sales Analysis

* Total sales by category
* Average spending by category
* Sales by payment method
* Sales by location
* Yearly sales
* Monthly sales
* Sales by day of week
* Sales by category and location

### 5. Product Analysis

* Top 10 items by quantity sold
* Top 10 items by revenue
* Item frequency analysis

### 6. Distribution & Correlation Analysis

* Quantity distribution
* Total spent distribution
* Price per unit vs. total spent
* Quantity vs. total spent
* Correlation matrix
* Numerical correlation heatmap

### 7. Discount Analysis

* Distribution of discount status
* Transaction count by discount status
* Average spending by discount status
* Total spending by discount status

## Key Data Quality Findings

The dataset contains missing values in several fields:

| Column             | Missing Values |
| ------------------ | -------------: |
| `Item`             |          1,213 |
| `Price Per Unit`   |            609 |
| `Quantity`         |            604 |
| `Total Spent`      |            604 |
| `Discount Applied` |          4,199 |

No duplicated rows were found in the dataset.

## Technologies

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn

## Project Structure

```text
retail-sales-analysis/
│
├── RetailSales.ipynb
├── retail_store_sales.csv
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/GovharOrujova/retail-sales-analysis.git
cd retail-sales-analysis
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook RetailSales.ipynb
```

## Requirements

```text
pandas
numpy
matplotlib
seaborn
jupyter
```

## Author

**Govhar Orujova**

📩 Email:
[govharorucova@outlook.com](mailto:govharorucova@outlook.com)

🌐 GitHub:
https://github.com/GovharOrujova

🔗 LinkedIn:
https://www.linkedin.com/in/govhar-orujova-64333b369/
