# Retail Sales Data Cleaning Project

## Project Overview
This project focuses on cleaning and preparing a retail sales dataset for data analysis.  
The raw dataset contained missing values and incomplete transaction records, which needed to be handled before any meaningful analysis could be performed.

The main goal of this project was to clean the data, document the decisions made during the process, and export a processed dataset that can be used for further analysis.

This is my first project related to data analytics.

---

## Dataset Description
The dataset contains retail transaction data with the following columns:

- Transaction ID  
- Transaction Date  
- Customer ID  
- Gender  
- Age  
- Product Category  
- Item  
- Price Per Unit  
- Quantity  
- Total Spent  
- Payment Method  
- Store Location  
- Discount Applied  

### Dataset Size
- Raw dataset: 12,575 rows  
- Cleaned dataset: 11,362 rows  

---

## Issues Found in the Raw Data
While exploring the dataset, the following issues were identified:

- Missing values in important columns such as:
  - Item
  - Price Per Unit
  - Quantity
  - Total Spent
- A large number of missing values in the Discount Applied column
- Incomplete transaction records that could affect analysis results

---

## Data Cleaning Steps

### Handling Missing Values
Rows with missing values in transaction-critical columns (Item, Price Per Unit, Quantity, and Total Spent) were removed.  
These fields are essential for sales calculations and could not be reliably filled without making unrealistic assumptions.

### Discount Applied Column
Missing values in the Discount Applied column were filled with `False`.

Assumption made:  
If a discount was not recorded, it was assumed that no discount was applied.

### Data Integrity
- No columns were removed
- Only necessary rows were dropped
- The focus was on keeping valid and complete transactions

---

## Final Result
- All missing values were handled
- The dataset is clean and consistent
- A processed CSV file was created for further analysis
- The final dataset can be used for exploratory data analysis or visualization tasks

---

## Tools Used
- Python  
- Pandas  
- Jupyter Notebook  

---