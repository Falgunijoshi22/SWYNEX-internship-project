# Transaction Data Cleaning and Transformation Using Python

## Project Overview

This project focuses on cleaning and transforming transaction data using Python and Pandas. The objective is to improve data quality and prepare the dataset for further analysis and visualization.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Dataset Description

The dataset contains transaction records with information such as transaction ID, product item, quantity, price per unit, total spending, payment method, location, and transaction date.

## Data Cleaning and Transformation

- Inspected dataset structure, column names, and data types.
- Identified missing values and invalid placeholder entries.
- Standardized `UNKNOWN` and `ERROR` values as missing values.
- Converted numeric columns to appropriate data types.
- Converted transaction dates to datetime format.
- Validated total spending using quantity and price per unit.
- Checked for duplicate rows and transaction IDs.
- Extracted month and year from transaction dates.
- Performed final data-quality checks.

## Project Outcome

The project demonstrates a structured approach to data cleaning and transformation, preparing transaction data for future exploratory data analysis, reporting, and visualization.

## How to Use

1. Clone or download this repository.
2. Install the required libraries using `pip install pandas numpy jupyter`.
3. Open `transaction_data_cleaning.ipynb` in Jupyter Notebook.
4. Update the dataset path if necessary and run the notebook cells.

## Author

Falguni Joshi 