# DecodeLabs Data Science Internship - Project 1

## Advanced EDA & Feature Engineering

This project focuses on transforming raw e-commerce data into a clean machine-learning-ready dataset.

## Objectives

- Perform Exploratory Data Analysis (EDA)
- Handle missing values using statistical imputation
- Detect and treat outliers using IQR and Z-score methods
- Create new predictive features

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset

The dataset contains customer order information including:

- Order details
- Customer information
- Product information
- Pricing
- Payment methods
- Order status

## Data Preprocessing

### Missing Values

Handled missing values in CouponCode using categorical imputation.

### Outlier Treatment

Detected numerical outliers using:

- Interquartile Range (IQR)
- Z-score

Outliers were capped instead of removed to preserve data.

## Feature Engineering

Created new features:

1. Price Per Item
2. Cart Fill Ratio
3. High Value Order Indicator
4. Coupon Usage Flag
5. Referral Feature

## Output

Generated cleaned dataset:

project_1_cleaned_dataset.csv

## Author

Tanmay Singh