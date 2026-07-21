# E-Commerce Exploratory Data Analysis (EDA)

This repository contains a Python-based Exploratory Data Analysis (EDA) project for an e-commerce dataset. The analysis focuses on extracting business insights, identifying sales trends, and detecting anomalies within customer orders.

## Features
- **Data Cleaning & Transformation:** Handles missing values (e.g., missing coupon codes) and generates new analytical columns like `Purchase_Ratio` and `Month`.
- **Basic Statistics:** Calculates key metrics such as mean, median, and count for quantities, unit prices, items in cart, and total prices.
- **Trend Analysis:** 
  - Identifies the top-performing products by total revenue.
  - Determines the most profitable marketing/referral sources.
- **Outlier Detection:** Utilizes the Interquartile Range (IQR) method to identify unusually high-value transactions.

## Dataset
The script requires an Excel dataset named `Dataset for Data Analytics 2 .xlsx`. The dataset should contain columns like `OrderID`, `Date`, `Product`, `Quantity`, `ItemsInCart`, `TotalPrice`, `CouponCode`, and `ReferralSource`.

## Prerequisites
To run this script, you need Python installed on your system along with the following libraries:
- `pandas`
- `numpy`
- `openpyxl` (for reading `.xlsx` files)

You can install the required packages using pip:
```bash
pip install pandas numpy openpyxl