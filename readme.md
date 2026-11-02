# Café Sales Data Analysis and Interactive Dashboard

## 1. Project Overview

This project focuses on analyzing café sales data to understand product performance, revenue trends, customer payment preferences, and sales patterns.

The project was completed as part of my **Data Analytics Internship at SWYNEX Technologies**. It covers the complete data analytics workflow, starting with raw data cleaning and preparation, followed by exploratory data analysis (EDA), visualization, and interactive dashboard development using Power BI.

## 2. Problem Statement

Understanding sales performance is essential for businesses to make informed decisions and improve their operations.

The objective of this project is to analyze café transaction data to identify popular products, evaluate revenue contribution, understand monthly sales trends, examine payment preferences, and compare sales performance.

The analysis aims to transform raw transaction data into meaningful insights that can help understand business performance and support data-driven decision-making.

## 3. Dataset Information

**Dataset Name:** Café Sales Dataset  
**Dataset Source:** [Add dataset source/link]

The dataset contains transaction-level information about café sales.

### Dataset Columns

| Column | Description |
|---|---|
| Transaction ID | Unique transaction identifier |
| Item | Name of the product purchased |
| Quantity | Number of units purchased |
| Price Per Unit | Price of one unit |
| Total Spent | Recorded transaction amount |
| Payment Method | Payment method used |
| Location | Transaction location |
| Transaction Date | Date of the transaction |

## 4. Tools and Technologies

- **Python:** Data cleaning, manipulation, and analysis
- **Pandas:** Data processing and analysis
- **NumPy:** Numerical operations
- **Matplotlib:** Data visualization
- **Jupyter Notebook:** Python development environment
- **Power BI Desktop:** Interactive dashboard development
- **GitHub:** Project documentation and version control

---

## 5. Task 1: Data Cleaning and Preparation

### Objective

To inspect, clean, and prepare the raw café sales dataset for further analysis.

### Cleaning Process

The following data cleaning steps were performed using Python:

- Inspected the dataset structure, columns, data types, and statistical information.
- Identified missing values and inconsistent entries.
- Replaced invalid placeholder values such as `UNKNOWN` and `ERROR` with missing values.
- Converted numerical columns, including Quantity, Price Per Unit, and Total Spent, into appropriate numeric data types.
- Converted the Transaction Date column into datetime format.
- Extracted additional date-related information, including Month and Year.
- Created a cleaned version of the dataset for further analysis.

**Output:** `cleaned_cafe_sales.csv`

The cleaned dataset was used as the input for Task 2 and Task 3.

---

## 6. Task 2: Exploratory Data Analysis (EDA)

### Objective

To explore the cleaned dataset, calculate important statistics, identify trends and patterns, and extract meaningful business insights.

### Analysis Performed

The following analyses were conducted using Python:

1. **Product-wise Quantity Analysis:** Identified the most popular products based on total quantity sold.
2. **Revenue Analysis:** Compared recorded revenue across different products.
3. **Monthly Revenue Analysis:** Examined monthly revenue trends to identify high-performing periods.
4. **Payment Method Analysis:** Analyzed transactions by payment method to understand payment preferences.
5. **Location-wise Revenue Analysis:** Compared revenue across different locations.
6. **Anomaly Detection:** Checked for invalid quantities, non-positive prices, and differences between recorded and calculated transaction totals.

### Visualizations Created

- Total Quantity Sold by Item
- Total Revenue by Item
- Monthly Revenue Trend
- Transactions by Payment Method
- Total Revenue by Location

### Key Business Insights

1. **Most Popular Product:** Juice recorded the highest quantity sold, indicating strong customer demand compared to the other products.

2. **Product-wise Revenue:** Based on the recorded revenue figures, Juice generated the highest revenue (3,373), closely followed by Coffee (3,368). Cookie recorded the lowest revenue (3,090).

3. **Monthly Revenue Trend:** June recorded the highest revenue among the analyzed months, indicating a peak in sales during this period.

4. **Product Performance Comparison:** Revenue figures across the eight products were relatively close, suggesting that revenue contribution was distributed across multiple products rather than being concentrated in just one.

---

## 7. Task 3: Interactive Dashboard Development Using Power BI

### Objective

To create an interactive dashboard that presents important sales metrics, visualizations, and business findings in a clear and accessible format.

### Dashboard Features

The Café Sales Performance Dashboard was developed using Power BI Desktop.

**Key Performance Indicators (KPIs):**

- **Total Revenue:** Displays the total recorded revenue.
- **Total Quantity Sold:** Shows the total number of units sold.
- **Average Spend:** Displays the average transaction value.

**Visualizations:**

1. **Quantity Sold by Item:** Compares the total quantity sold across different products.
2. **Total Revenue by Item:** Displays revenue contribution by individual products.
3. **Payment Method Analysis:** Shows the distribution of transactions across payment methods.
4. **Quantity by Day:** Displays quantity trends across different days of the week.

**Interactive Filters (Slicers):**

- Month selection
- Item name selection

These slicers allow users to filter the dashboard and explore sales performance for specific months and products.

### Dashboard Preview

![Café Sales Power BI Dashboard]
![Project Screenshot]("C:\Users\falgu\OneDrive\Pictures\Screenshots\Screenshot 2026-11-02 131935.png")


## 8. Task 4: Final Project Documentation

### Objective

To consolidate the complete data analytics workflow into a single documented project and make the work accessible through GitHub.

This final stage brings together:

- Raw and cleaned datasets
- Data cleaning and preparation notebook
- Exploratory data analysis notebook
- Power BI dashboard and its visual representation
- Key business insights and project conclusion


## 9. Conclusion

This project provided practical experience in the complete data analytics workflow, from data cleaning and preparation to exploratory analysis and interactive dashboard development.

Using Python and Power BI, I explored café sales data to understand product performance, revenue contribution, monthly sales trends, and payment preferences.

The project strengthened my understanding of data manipulation, statistical analysis, data visualization, and dashboard development. It also demonstrated how raw data can be transformed into meaningful insights that support better business understanding and decision-making.

---

## 10. Internship Information

**Organization:** SWYNEX Technologies  
**Domain:** Data Analytics  
**Project:** Café Sales Data Analysis and Interactive Dashboard

## 11. Author
Falguni Joshi
GitHub: [Your GitHub Profile](https://github.com/Falgunijoshi22)
