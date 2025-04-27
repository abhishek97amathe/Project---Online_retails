# Project-Online_retails
 The dataset is a comprehensive transaction record of all sales made by a UK-based online retailer from December 1, 2010, to December 9, 2011. The project focuses on preparing the dataset for analysis by handling missing values, removing duplicates, detecting outliers, and creating visualizations to uncover insights. 

## About the Project
This project involves cleaning and performing exploratory data analysis (EDA) on an e-commerce dataset. The dataset contains information about online retail transactions, including invoice numbers, product descriptions, quantities, unit prices, and customer IDs.

---

## Steps Performed

### 1. Data Cleaning
- **Removed Duplicates**: Identified and removed duplicate rows to ensure data consistency.
- **Handled Missing Values**:
  - Dropped rows with missing values in critical columns like `InvoiceNo`.
  - Checked for missing values in other columns and handled them appropriately.
- **Converted Data Types**:
  - Converted `InvoiceNo` to numeric, coercing non-numeric values to `NaN`.
  - Dropped rows with `NaN` in `InvoiceNo` and converted it to integers.
- **Reset Index**: Reset the index of the DataFrame after cleaning.

### 2. Exploratory Data Analysis (EDA)
- **Descriptive Statistics**:
  - Used `df.describe()` to generate summary statistics for numerical columns.
  - Checked the shape of the dataset and column data types.
- **Outlier Detection**:
  - Used the Interquartile Range (IQR) method to identify outliers in columns like `Quantity` and `UnitPrice`.
  - Visualized outliers using boxplots.
- **Data Visualization**:
  - Created boxplots for `Quantity` and `UnitPrice`.
  - Counted occurrences of unique values in columns like `Description` and `Country`.
- **New Features**:
  - Created a new column `sales` by multiplying `Quantity` and `UnitPrice`.

## Outcomes of EDA
### 1.Data Cleaning:
Removed duplicate rows to ensure data consistency.
Handled missing values by dropping rows with critical missing data (e.g., InvoiceNo).
Converted data types (e.g., InvoiceNo to integers) for proper analysis.
Outlier Detection:

Identified outliers in key numerical columns like Quantity and UnitPrice using the Interquartile Range (IQR) method.
Visualized outliers using boxplots to understand their impact on the dataset.
Feature Engineering:

Created a new column sales by multiplying Quantity and UnitPrice to analyze revenue generated per transaction.
Descriptive Statistics:

Generated summary statistics for numerical columns to understand the central tendency, spread, and distribution of the data.
Analyzed the shape and structure of the dataset.
Insights from Visualizations:

Used boxplots to visualize the distribution of Quantity and UnitPrice.
Counted the occurrences of unique values in categorical columns like Description and Country to identify popular products and customer demographics.
Dataset Preparation:

Cleaned and prepared the dataset for further analysis or modeling by ensuring data consistency, removing outliers, and handling missing values.

### 2.Key Insights
Identified products with unusually high or low quantities and prices.
Highlighted countries with the most transactions, providing insights into customer demographics.
Prepared the dataset for revenue analysis by creating the sales column.
