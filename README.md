# Sales Data Analysis

## Overview

This project analyzes sales data to extract meaningful market and business insights. The goal is to understand customer behavior, identify sales trends, and gain valuable information for decision-making. Key business questions were explored to uncover trends, customer preferences, and product performance.

![screenshot-localhost_8888-2025 03 01-15_09_14](https://github.com/user-attachments/assets/e0536100-b2d7-4b58-b9ac-e31ffc506fb5)

### Project Goals
- Analyze sales data to identify trends in customer purchasing behavior.
- Understand the performance of different products and how they are bought together.
- Evaluate sales performance and identify outliers.
- Identify patterns in order values and customer behavior across time and product categories.

### Data Overview

The dataset consists of sales transactions with the following columns:

- Order ID: Unique identifier for each order.
- Product: The name of the product purchased.
- Quantity Ordered: The number of units ordered.
- Price Each: The price per unit of the product.
- Order Date: The date and time of the order.
- Purchase Address: The delivery address for the order.
- Month: The month in which the order was placed.
- Sales: The total sales amount for each order.
- City: The city where the order was placed.
- Hour: The hour of the day when the order was placed.

### Methodology

1. Data Cleaning:
- Handled missing values, duplicates, and ensured that sales figures were computed correctly.
- Converted the 'Order Date' to datetime format and ensured that 'Quantity Ordered' and 'Price Each' were positive.

2. Analysis:
- Used groupby(), lambda functions, and Counter for analyzing product pairings and frequency.
- Performed various aggregations (e.g., summing sales, counting orders) to find trends.

3. Visualization:
- While no visualizations were included in the initial analysis, trends such as seasonal sales, sales by hour, and product pairings could be further analyzed through visualizations using tools like Matplotlib or Seaborn.

### Analysis Performed

1. Customer Behavior & Purchasing Patterns:
- Quantity Ordered vs. Price Each: Analyzed to see if customers prefer purchasing expensive items in bulk or individually.
- Product Pairings: Investigated which products are often purchased together by identifying duplicate Order IDs.
- Product Distribution: Analyzed which products are popular in different cities.
- Weekday vs. Weekend Orders: Compared orders placed on weekdays and weekends to understand consumer behavior.

2. Market & Business Insights:
- Product Category Performance: Classified products into categories and analyzed sales by category.
- Seasonal Sales Trends: Compared sales across different months to identify seasonal trends.
- Price Range Performance: Categorized products into different price ranges and analyzed which range contributes the most to revenue.
- Outlier Detection: Identified extreme high and low sales transactions to understand outliers.
- Average Order Value (AOV): Calculated the average revenue per order.
- Unique Customers: Estimated the number of unique customers based on purchase addresses.

### Key Findings

- Customer Purchasing Behavior: Most customers purchase only one item per transaction, with a wide range of product prices.
- Sales Trends: Sales fluctuate by month, suggesting seasonal demand.
- Peak Hours: Peak purchasing activity occurs in the afternoon, specifically around 2-3 PM. The peak hour for orders is around 7 PM.
- Product Pairings: Phones are often bought alongside accessories like charging cables and headphones. This indicates that customers prefer to buy compatible products together.
- Order Frequency: There is a notable distinction in orders between weekdays and weekends, with a higher number of orders during weekdays.
- Outliers: There are a few high sales outliers in the data, but no significant low sales outliers were identified.
- Average Order Value (AOV): The average order value is approximately $193.15, which provides insight into customer spending.

### Source

![Sales Data Analysis Datset found at Kaggle.](https://www.kaggle.com/datasets/beekiran/sales-data-analysis)
