# Exploratory Data Analysis for Instacart

## Overview
This project analyzes Instacart order data to understand customer purchasing behavior, basket composition, and reorder patterns. The analysis follows a full exploratory workflow, moving from raw data inspection through cleaning, transformation, and insight generation.

The focus is not only on producing results, but on demonstrating the ability to work with real-world, multi-table datasets and translate quantitative findings into meaningful, business-relevant observations.

---

## Objective
The goal of this analysis is to uncover patterns in customer ordering behavior, including:
- When customers are most likely to place orders
- How frequently customers return to reorder
- Which products are most frequently purchased and reordered
- How basket size and composition vary across orders

---

## Data Source
This project uses the **Instacart Online Grocery Basket Analysis** dataset, publicly available on Kaggle:

https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis

Due to file size limitations, the dataset is not included in this repository.  
To run this project locally, download the dataset and place the CSV files in a `datasets/` directory.

---

## Dataset Structure
The analysis uses multiple related tables:
- **orders** — order-level information (user, order number, timing)
- **products** — product metadata
- **aisles** — aisle-level categorization
- **departments** — department-level categorization
- **order_products** — links products to orders, including reorder flags  
  *(constructed by combining prior and train datasets)*

---

## Workflow

### Data Inspection
- Reviewed dataset structure using `.info()` and `.head()`
- Identified missing values and structural inconsistencies

### Data Cleaning
- Investigated and handled missing values contextually
- Removed duplicates and standardized fields
- Validated assumptions about time-based variables

### Data Transformation
- Merged multiple tables using shared keys
- Reshaped and filtered data for analysis
- Constructed a unified `order_products` dataset

### Analysis
- Evaluated order patterns by hour and day
- Analyzed time between orders
- Measured customer activity distribution
- Calculated product-level reorder rates

### Visualization
- Visualized temporal ordering patterns
- Examined basket size distributions
- Highlighted trends in customer behavior

---

## Key Insights
- Customer activity follows a strong daily cycle, with peak ordering during mid-morning to afternoon hours
- Weekly ordering patterns suggest routine shopping behavior, with higher activity at the beginning of the week
- Reordering behavior is highly concentrated in a subset of frequently purchased items
- Produce and perishable goods dominate both purchase frequency and reorder rates
- Most orders are relatively small, with a long tail of larger baskets

---

## Tools and Technologies
- Python
- Pandas
- NumPy
- Matplotlib

---

## How to Run
1. Clone this repository
2. Download the dataset from Kaggle (link above)
3. Create a `datasets/` folder in the project directory
4. Place all CSV files inside the `datasets/` folder
5. Open the notebook in Jupyter Notebook, JupyterLab, or VS Code
6. Run all cells sequentially

---

## Notes
- This project has been adapted for portfolio presentation and cleaned of instructional and environment-specific elements
- The workflow reflects practical data analysis techniques applied to real-world structured data

---

## Author
Michael
