Data Cleaning and Preprocessing Task
Dataset

Source: Mall Customer Segmentation Data from Kaggle
Description: Contains customer information like Gender, Age, Annual Income, and Spending Score, suitable for practicing data cleaning.

Cleaning Steps

Missing Values: Identified missing values using .isnull(). Filled numeric columns with median and categorical columns (e.g., Gender) with mode.
Duplicates: Removed duplicate rows using .drop_duplicates().
Text Standardization: Converted 'Gender' to lowercase and standardized values (e.g., 'm' to 'male', 'f' to 'female').
Column Names: Renamed columns to lowercase with underscores for consistency.
Data Types: Ensured 'age' is integer type. (No date columns in this dataset, so no datetime conversion applied.)
Outliers: Detected outliers in numeric columns (e.g., Annual Income, Spending Score) using IQR method and capped them.
Output: Saved cleaned dataset as Mall_Customers_Cleaned.csv and generated this README.

Files

data_cleaning.py: Python script performing the cleaning steps.
Mall_Customers.csv: Original dataset (not included here; download from Kaggle).
Mall_Customers_Cleaned.csv: Cleaned dataset.
README.md: This summary file.

Tools Used

Python 3.x
Pandas library

How to Run

Download Mall_Customers.csv from Kaggle.
Place it in the same directory as data_cleaning.py.
Run python data_cleaning.py to generate the cleaned dataset and README.

Notes

No paid tools were used.
The script assumes the dataset has columns like 'Gender', 'Age', 'Annual Income (k$)', and 'Spending Score (1-100)'.
Adjust the script if your dataset has different column names or additional issues.

