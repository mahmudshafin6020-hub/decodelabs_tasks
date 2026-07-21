Features and Data Processing Steps: 

The script performs the following data cleaning operations sequentially:

1. Data Loading & Inspection:
    -Loads the raw dataset (Dataset for Data Analytics, project 1 - Sheet1.csv). Calculates and prints the initial total row count.

2. Missing Value Identification:
    -Scans the dataset for null or missing values and reports the exact count per column (e.g., identifying missing CouponCode entries).

3. Duplicate Removal:
Identifies and completely removes identical duplicate rows to prevent skewed analysis.

   -Data Formatting & Standardization:

   -Dates: Converts the Date column into proper Pandas datetime objects.

   -Text: Cleans categorical and text columns (Product, PaymentMethod, OrderStatus, CouponCode, ReferralSource) by stripping accidental trailing/leading whitespaces and standardizing the text to Title Case.

   -Missing Text Handling: Safely reverts accidental 'Nan' strings back to true np.nan values.

   -Numeric Values: Forces Quantity, UnitPrice, and TotalPrice into strict numeric formats, coercing any accidental text anomalies into NaN.


4.Data Export:
   -Exports the final, pristine dataset as Cleaned_Dataset.csv without the index column.