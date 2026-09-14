# Online Retail Data Analysis

This project analyzes an online retail transaction dataset to uncover sales patterns, customer behavior, and revenue opportunities. The analysis is implemented in a Jupyter Notebook and includes data cleaning, exploratory data analysis, and business insight generation.

## Project Goals

- Understand the structure and quality of the retail dataset
- Clean invalid or incomplete records before analysis
- Explore product, customer, and regional sales trends
- Identify the most valuable products and customers
- Use RFM analysis to understand customer value and recency
- Summarize insights that can support business decisions

## Dataset

The project uses the file `online_retail.csv`.

Columns include:
- `InvoiceNo`
- `StockCode`
- `Description`
- `Quantity`
- `InvoiceDate`
- `UnitPrice`
- `CustomerID`
- `Country`

This dataset contains online retail transactions and is commonly used for customer segmentation and sales analytics.

## Data Cleaning Process

The notebook performs the following steps:

1. Load the retail dataset
2. Check for missing values and duplicate rows
3. Detect negative quantities and invalid prices
4. Remove rows with missing `CustomerID`
5. Remove duplicate records
6. Filter out negative `Quantity` and zero/negative `UnitPrice`
7. Convert `InvoiceDate` to datetime format
8. Create a new `TotalPrice` column using:
   `TotalPrice = Quantity * UnitPrice`
9. Remove outliers using IQR-based filtering

## Exploratory Data Analysis

The analysis covers:

- Distribution of numerical variables (`Quantity`, `UnitPrice`, `TotalPrice`)
- Top-selling products by quantity
- Top products by revenue
- Sales by country
- Monthly sales trend
- Revenue by hour of the day
- Customer spending distribution
- Correlation between numeric variables

## Business Insight Analysis

Additional analyses include:

- Top customers by revenue
- RFM (Recency, Frequency, Monetary) analysis
- Customer monetary value distribution
- Correlation between RFM metrics
- Revenue by day of the week
- Top 10 products contributing to revenue

## Project Files

- `online_retail.csv` - raw transaction dataset
- `test (1).ipynb` - main data analysis notebook
- `LAPORAN AKHIR.pdf` - final report document
- `README.md` - project documentation

## Requirements

To run the notebook, install the following Python packages:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## How to Run

1. Open the project folder
2. Launch Jupyter Notebook or VS Code notebook interface
3. Open `test (1).ipynb`
4. Run the cells sequentially

## Example Insights

This project is designed to help answer questions such as:

- Which products generate the most revenue?
- Which countries contribute the most sales?
- What is the sales trend over time?
- Which customers are the highest-value buyers?
- How can RFM segmentation support marketing and retention strategies?

## Summary

This project demonstrates a complete workflow for an e-commerce sales dataset: cleaning, exploring, analyzing, and deriving actionable business insights. It is suitable for practice in data analytics, customer segmentation, and retail performance analysis.
