# Zepto Portfolio Data Analytics

## Project Overview
This project analyzes a Zepto e-commerce dataset to uncover insights about product pricing, discounts, inventory, and category-wise trends. The dataset was sourced from Kaggle and mimics real-world e-commerce inventory data.

## Dataset Description
- Each row represents a unique SKU (Stock Keeping Unit) for a product.
- Duplicate product names exist because the same product may appear in different package sizes, weights, discounts, or categories.

## Key Tasks Performed
- Extracted and explored data from **PostgreSQL**, performing data quality checks for nulls, duplicates, and inconsistencies:
  - Counted total records and viewed sample data to understand structure
  - Checked for null values and distinct product categories
  - Compared in-stock vs out-of-stock products
  - Detected duplicate product names representing multiple SKUs
- Cleaned and transformed data:
  - Removed rows with zero MRP or discounted selling price
  - Converted `mrp` and `discountedSellingPrice` from paise to rupees
- Conducted SQL-based analysis to derive actionable business insights:
  - Identified top 10 best-value products based on discount percentage
  - Highlighted high-MRP products that are out of stock
  - Calculated potential revenue per category
  - Filtered expensive products (MRP > ₹500) with minimal discounts
  - Ranked top 5 categories offering highest average discounts
  - Calculated price per gram for value-for-money analysis
  - Grouped products by weight into Low, Medium, and Bulk categories
  - Measured total inventory weight per product category

## Tools & Technologies
- **Database:** PostgreSQL  
- **Languages:** SQL  
- **Analysis & Reporting:** Excel

## Impact
- Provided insights into pricing, discount trends, inventory distribution, and product value metrics to support data-driven decision-making.
