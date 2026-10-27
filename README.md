# Retail Data Cleaning and Sales Analysis

## Project Overview
This project analyzes an online retail transaction dataset using Python. It focuses on data cleaning, exploratory data analysis (EDA), and visualization to identify sales trends, popular products, and leading markets.

## Tools and Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- Visual Studio Code

## Dataset
The dataset contains online retail transactions with information such as invoice number, product code, product description, quantity, invoice date, unit price, customer ID, and country.

## Data Cleaning
- Identified missing values.
- Removed exact duplicate records.
- Removed rows with missing product descriptions.
- Converted invoice dates to datetime format.
- Investigated negative quantities and prices.
- Created a `Sales` column using `Quantity × UnitPrice`.
- Preserved missing customer IDs and zero-price transactions for further analysis.

## Key Findings
- **Cleaned records:** 535,185
- **Duplicate records remaining:** 0
- **Invalid dates remaining:** 0
- **Total calculated sales:** 9,748,131.07
- **Top country by sales:** United Kingdom
- **Top product by quantity sold:** PAPER CRAFT, LITTLE BIRDIE

## Visualizations
1. Monthly sales trend.
2. Top 10 products by quantity sold.
3. Top 10 countries by sales.

## Project Structure
```text
internship/
├── data/
│   └── online_retail.csv
├── notebooks/
│   └── data_cleaning_visualization.ipynb
├── outputs/
│   └── cleaned_online_retail.csv
├── requirements.txt
└── README.md
```

## How to Run
1. Install Python.
2. Install the required packages using `pip install -r requirements.txt`.
3. Open the notebook in Jupyter or VS Code.
4. Run the notebook cells in order.

## Limitations
The analysis uses transaction-level data. Negative quantities may represent returns or cancellations, and calculated sales include their negative values. Missing customer IDs limit customer-level analysis. Findings should be interpreted in light of these data-cleaning decisions.
