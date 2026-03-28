# Instacart Data Analysis

## Overview
Exploratory data analysis of Instacart order data using Python (Pandas). The project focuses on cleaning datasets, merging multiple tables, and analyzing customer purchasing behavior and reorder patterns.

## Objective
Identify trends in customer orders, including:
- When customers place orders
- Which products are reordered most frequently
- How ordering behavior varies across users

## Dataset
The analysis uses multiple related datasets:
- **orders** — order-level information (time, user, order number)
- **products** — product details
- **order_products** — links products to orders, including reorder status

## Key Steps
- Data inspection and cleaning
  - handled missing values
  - removed duplicates
  - standardized column names
- Data transformation
  - merged datasets using common keys
  - filtered and reshaped data
- Analysis
  - grouped and aggregated data
  - calculated reorder rates
  - examined time-based trends
- Visualization
  - plotted order frequency by hour and day

## Key Insights
- Customer orders follow clear daily patterns, with peak activity at specific hours
- Certain products show consistently high reorder rates
- Reordering behavior varies across users and product categories

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib

## How to Run
1. Clone the repository
2. Open the notebook in Jupyter Notebook or JupyterLab
3. Run all cells in order

## Notes
- This project was completed as part of an AI/ML bootcamp

## Author
Michael
