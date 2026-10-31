# Cafe sales Data Cleaning and Preparation Using Python

**Internship:** Data Analytics Internship — Task 1  
**Organization:** SWYNEX Technologies  
**Project Type:** Data Cleaning and Transformation  
**Tools:** Python, Pandas, NumPy, Jupyter Notebook

## 1. Project Overview

This project was completed as part of Task 1 of my Data Analytics Internship at SWYNEX Technologies. The objective was to clean and prepare a cafe sales dataset using Python so that it could be used reliably for further analysis and visualization.

The dataset contains transaction-level information, including product items, quantities, prices, total spending, payment methods, locations, and transaction dates.

The project focuses on identifying data-quality issues, standardizing invalid values, converting data types, validating transaction totals, and creating useful date-based features.

## 2. Project Objectives

- Inspect the dataset and understand its structure.
- Identify missing values and invalid entries.
- Standardize inconsistent placeholder values.
- Convert columns to appropriate data types.
- Validate transaction totals using quantity and price per unit.
- Extract month and year from transaction dates.
- Perform final data-quality checks.
- Export the cleaned dataset for further analysis.

## 3. Dataset Description

The dataset contains the following columns:

| Column | Description |
|---|---|
| `Transaction ID` | Unique identifier assigned to a transaction |
| `Item` | Product associated with the transaction |
| `Quantity` | Number of units purchased |
| `Price Per Unit` | Price of one unit of the product |
| `Total Spent` | Recorded total spending for the transaction |
| `Payment Method` | Method used to make the payment |
| `Location` | Transaction or purchase location |
| `Transaction Date` | Date on which the transaction occurred |

The dataset contains both numerical and categorical data, along with transaction dates that can support time-based analysis.

## 4. Tools and Technologies

- **Python:** Programming language used for data cleaning.
- **Pandas:** Used to load, inspect, clean, transform, and export tabular data.
- **NumPy:** Used to represent missing values and support data preparation.
- **Jupyter Notebook:** Used to execute Python code and document the workflow.

## 5. Initial Data Quality Findings

During the initial inspection, several data-quality issues were identified.

### Missing Values

The dataset contained missing values (`NaN`) in multiple columns, including:

- Item
- Quantity
- Price Per Unit
- Total Spent
- Payment Method
- Location
- Transaction Date

### Invalid Placeholder Values

The dataset also contained placeholder strings such as `UNKNOWN` and `ERROR`. These values were not valid transaction details and needed to be handled before analysis.

### Data Type Issues

Some numerical fields and transaction dates required conversion to appropriate data types for calculations and date-based operations.

### Transaction Validation

Recorded transaction totals needed to be checked against the expected total calculated from quantity and price per unit.

## 6. Data Cleaning Process

### Step 1: Data Inspection

- Loaded the original CSV dataset using Pandas.
- Inspected the first rows using `head()`.
- Checked the number of rows and columns using `shape`.
- Examined column data types and non-null counts using `info()`.
- Counted missing values using `isnull().sum()`.

### Step 2: Standardizing Invalid Values

Replaced the exact placeholder strings `UNKNOWN` and `ERROR` with missing values (`NaN`) using Pandas and NumPy.

This made invalid entries easier to identify and handle consistently.

### Step 3: Converting Numeric Columns

Converted the following columns to numeric data types:

- `Quantity`
- `Price Per Unit`
- `Total Spent`

Invalid numeric entries were converted to missing values for further investigation.

### Step 4: Date Conversion

Converted `Transaction Date` into a datetime data type using `pd.to_datetime()`.

Invalid date entries were converted to `NaT`, allowing date operations to be performed consistently.

### Step 5: Creating Date-Based Features

Extracted additional information from the transaction date:

- `Month`: Month name associated with the transaction.
- `Year`: Year associated with the transaction.

These features can be used for monthly and yearly transaction analysis.

### Step 6: Calculating and Validating Transaction Totals

Created a calculated total using:

`Calculated Total = Quantity × Price Per Unit`

Compared the calculated values with the recorded `Total Spent` values to identify missing totals and potential inconsistencies.

Missing totals can be filled from the calculated values when the calculation is valid and the business rule has been confirmed.

### Step 7: Data Quality Validation

Performed checks for:

- Remaining missing values.
- Duplicate rows.
- Repeated transaction IDs.
- Invalid quantities and prices.
- Differences between recorded and calculated totals.
- Final column data types.

Potential duplicate records and inconsistent totals should be investigated before any records are removed or overwritten.

## 7. Data Transformation

The following transformations were performed or prepared as part of the workflow:

- Standardization of invalid placeholder values.
- Conversion of numerical columns into usable numeric formats.
- Conversion of transaction dates into datetime format.
- Extraction of month and year features.
- Calculation of expected transaction totals.
- Preparation of the cleaned dataset for export.

## 8. Key Findings and Learning Outcomes

### Data Quality Findings

- The original dataset contained missing values across multiple transaction fields.
- Placeholder values such as `UNKNOWN` and `ERROR` required standardization.
- Some transaction totals were missing or invalid and could be checked using quantity and unit price.
- Invalid transaction dates needed to be identified before time-based analysis.

### Learning Outcomes

Through this project, I gained practical experience in:

- Inspecting real-world tabular data using Pandas.
- Identifying missing values and inconsistent entries.
- Converting data types and handling invalid values.
- Creating date-based features.
- Validating derived numerical values.
- Documenting a structured data-cleaning workflow.

**Note:** This project focuses on data cleaning and preparation. Business insights such as highest-selling products, revenue trends, and preferred payment methods require additional exploratory data analysis.

## 9. Repository Structure

```text
python-transaction-data-cleaning/
│
├── README.md
├── transaction_data_cleaning.ipynb
├── data/
│   └── cleaned_transactions.csv
└── .gitignore
```

- `README.md` — Project overview, methodology, findings, and instructions.
- `transaction_data_cleaning.ipynb` — Jupyter Notebook containing the Python workflow, code, and outputs.
- `data/cleaned_transactions.csv` — Exported cleaned dataset, if included and permitted for redistribution.
- `.gitignore` — Specifies files and folders that should not be tracked by Git.

The repository structure may vary depending on which files are included.

## 10. How to Run the Project

### Prerequisites

Install Python and Jupyter Notebook, then install the required libraries:

```bash
pip install pandas numpy jupyter
```

### Steps

1. Clone or download this repository.
2. Place the original dataset in the appropriate project directory if it is not included.
3. Open `transaction_data_cleaning.ipynb` in Jupyter Notebook.
4. Update the CSV file path if necessary.
5. Run the notebook cells sequentially to reproduce the workflow.

## 11. Project Outcome

The project establishes a structured process for cleaning and transforming transaction data using Python. It prepares the dataset for subsequent exploratory data analysis, reporting, and visualization, subject to review of any remaining data-quality issues.

## Task 2: Exploratory Data Analysis (EDA)

### Objective
To perform Exploratory Data Analysis on the cleaned café sales dataset to identify sales trends, product performance, customer payment preferences, and location-wise revenue patterns.

### Analysis Performed

The cleaned dataset (`cleaned_cafe_sales.csv`) was used for the following analysis:

- **Product Performance:** Analyzed total quantity sold by each item to identify popular products.
- **Revenue Analysis:** Compared recorded revenue across different products to identify major revenue contributors.
- **Monthly Sales Trends:** Examined monthly revenue to understand changes in sales over time.
- **Payment Method Analysis:** Analyzed transaction counts and revenue by payment method to understand payment preferences.
- **Location-wise Sales:** Compared revenue across locations to evaluate sales performance.
- **Anomaly Detection:** Checked for invalid quantities, non-positive prices, and differences between recorded and calculated transaction totals.

### Visualizations

The following charts were created using Matplotlib:

1. Total Quantity Sold by Item
2. Total Revenue by Item
3. Monthly Revenue Trend
4. Transactions by Payment Method
5. Total Revenue by Location

### Key Business Insights

The analysis focused on extracting the following business insights:

- Identifying the most popular products based on quantity sold.
- Finding which products contribute the highest recorded revenue.
- Understanding monthly revenue fluctuations.
- Identifying the most frequently used payment methods.
- Comparing sales performance across different locations.
- Highlighting unusual transaction records that may require further investigation.

### Outcome

Completed exploratory analysis of the cleaned café sales dataset using Python. Generated visualizations, examined sales patterns, and identified potential business insights to support better understanding of café sales performance.
## 12. Acknowledgment

This project was completed as part of Task 1 of my Data Analytics Internship at **SWYNEX Technologies**.

The project helped strengthen my practical understanding of Python-based data cleaning, transformation, and validation.
