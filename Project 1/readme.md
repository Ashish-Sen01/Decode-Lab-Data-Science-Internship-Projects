# Advanced EDA & Feature Engineering

## Overview

This project focuses on cleaning and analyzing an e-commerce dataset. The objective was to transform raw data into a machine-learning-ready dataset through data cleaning, outlier analysis, and feature engineering.

## Tasks Completed

### Missing Value Handling
- Filled categorical missing values with appropriate replacements.
- Missing values in the `CouponCode` column were filled with `NoCoupon` to represent orders without a coupon.

### Data Formatting & Consistency
- Rounded values in the `TotalPrice` column to 2 decimal places.
- This was done to eliminate floating-point precision artifacts (e.g., `927.6600000000001`) and improve the readability and consistency of monetary values.

### Outlier Analysis
- Detected outliers using the IQR (Interquartile Range) method.
- Outliers were found in the `TotalPrice` column.
- After inspection, these values were identified as genuine high-value transactions and were retained.

### Feature Engineering
Created three new features:

| Feature | Description
|----------|------------|
| CouponUsed | Indicates whether a coupon was used (0 = No, 1 = Yes) |
| CartPurchaseRate | Ratio of purchased items to items added to cart |
| OrderQuarter | Quarter in which the order was placed (Q1–Q4) |

## Key Insights
- Coupon usage patterns were analyzed.
- Most used payment methods were identified.
- Top 5 best-selling products were determined.
- Quarter-wise sales performance was evaluated.
- Top most-used coupon codes were identified.

## Technologies Used
- Python
- Pandas
- NumPy
- Jupyter Notebook

## Output
- Cleaned Dataset
- Feature Engineered Dataset
- Exploratory Data Analysis (EDA)

## Author
**Ashish Kumar Sen**  
Data Science Intern at Decode Labs