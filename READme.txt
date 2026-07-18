# Supply Chain Data Analysis (DataCo Dataset)

## Overview
This notebook performs exploratory data analysis on the DataCo Supply Chain dataset, covering data cleaning, visualization, and business insight extraction related to sales, profit, shipping performance, and customer/product trends.

## Dataset
- **Source**: DataCo Supply Chain Dataset
- **Format**: CSV (encoding: latin1)
- Contains order-level records including sales, pricing, discounts, profit, shipping details, customer information, and product/category data.

## What this notebook covers

### 1. Data Cleaning
- Converted currency-formatted columns (e.g., `$1,234`) to proper numeric types
- Converted order and shipping date columns to datetime
- Cast ID columns to integer types and categorical columns (e.g., Delivery Status, Market, Shipping Mode) to `category` dtype
- Cleaned column names (stripped whitespace, replaced spaces with underscores)
- Handled missing values using context-appropriate methods (mode, median, constant fill)
- Removed redundant columns and checked for duplicate records

### 2. Exploratory Data Analysis
- Checked data shape, structure, and null value distribution (including a missing-value heatmap)
- Outlier detection using boxplots across key numeric columns
- Distribution analysis (histograms) for sales and other numeric features
- Correlation analysis between numeric features (correlation heatmap)

### 3. Visualization
- Sales distribution and category-wise sales comparisons
- Sales vs. profit per order (scatter plot)
- Discount vs. profit relationship
- Delivery status vs. late delivery risk
- Sales by shipping mode, customer segment, and month

### 4. Business Insights
- Identified top-selling products, top loss-making products, and top customers by sales
- Compared sales performance across categories, countries, and regions
- Analyzed the relationship between order discounts and profit per order
- Assessed average delivery time and late delivery risk by shipping mode and delivery status
- Reviewed monthly sales trends and sales distribution by customer segment

## Tools & Libraries
- Python: Pandas, NumPy
- Visualization: Matplotlib, Seaborn, Plotly
