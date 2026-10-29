# YuvaIntern-Data-Science-Task-6
Week 6 Integrative Capstone Project – Retail Sales Analysis, Exploratory Data Analysis, Customer Segmentation using K-Means, and Sales Prediction using Random Forest Regression with Python.

## Retail Sales Analysis and Customer Segmentation Using Python

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-150458)
![Scikit Learn](https://img.shields.io/badge/ML-Scikit--learn-orange)
![Project](https://img.shields.io/badge/Project-Data%20Science-green)

## Project Overview

This repository contains my Week 6 Integrative Capstone Project completed as part of the YuvaIntern Data Science program.

The project focuses on analyzing online retail transaction data to understand sales performance, explore customer purchasing patterns, perform customer segmentation, and develop a baseline sales prediction model using Python and machine learning techniques.

The project integrates data cleaning, exploratory data analysis, feature engineering, unsupervised learning, regression modeling, and business insights into one workflow.

## Project Objectives

- Load, inspect, and preprocess online retail transaction data.
- Identify missing values, duplicate records, and data quality issues.
- Perform Exploratory Data Analysis (EDA).
- Analyze sales trends across months, products, and countries.
- Create customer-level purchasing features.
- Segment customers using the K-Means clustering algorithm.
- Build a baseline sales prediction model using Random Forest Regression.
- Evaluate model performance using regression metrics.
- Generate meaningful business recommendations.

## Dataset

**Dataset:** `online_retail_cleaned.csv`

The dataset contains online retail transaction information.

Key fields used in the analysis include:

| Column | Description |
|---|---|
| InvoiceNo | Transaction or invoice identifier |
| CustomerID | Customer identification number |
| Quantity | Number of units purchased |
| UnitPrice | Price per unit |
| InvoiceDate | Transaction date and time |
| Description | Product description |
| Country | Country associated with the transaction |

The analysis uses the columns available in the supplied dataset.

## Technologies and Libraries

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine learning
- **Jupyter Notebook** – Interactive development environment

## Project Workflow

### 1. Data Loading and Inspection
- Loaded the retail dataset using Pandas.
- Examined the dataset structure and sample records.
- Checked data types, missing values, and duplicate records.

### 2. Data Cleaning and Preprocessing
- Reviewed missing values and duplicate records.
- Converted InvoiceDate into datetime format.
- Prepared transaction data for further analysis.

### 3. Feature Engineering

Created the following features:

- TotalSales
- InvoiceYear
- InvoiceMonth
- InvoiceDay
- InvoiceWeekday
- InvoiceHour

Total sales were calculated using:

`TotalSales = Quantity × UnitPrice`

### 4. Exploratory Data Analysis (EDA)

Performed analysis to understand:

- Monthly sales trends.
- Top-performing products.
- Country-wise sales performance.
- Customer purchasing patterns.

### 5. Customer Segmentation Using K-Means

Applied K-Means clustering to group customers based on:

- TotalSpending
- TotalQuantity
- NumberOfInvoices

StandardScaler was used to standardize the selected numerical features before clustering.

The model was configured to generate three customer clusters.

### 6. Sales Prediction Using Random Forest Regression

Developed a baseline Random Forest Regression model to predict transaction sales using available date-related features.

The model was evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### 7. Business Insights

The analysis provides a foundation for:

- Understanding customer purchasing behavior.
- Exploring high-spending and frequent-purchase customer groups.
- Monitoring retail sales patterns.
- Supporting customer retention and inventory planning strategies.

## Project Structure

```text
YuvaIntern-Data-Science-Task-6/
│
├── Task6_Integrative_Capstone.ipynb
├── Task6_Integrative_Capstone_Report.docx
├── README.md
├── requirements.txt
├── .gitignore
│
└── outputs/
    ├── task6_cleaning_summary.csv
    ├── task6_customer_segments.csv
    ├── task6_segment_summary.csv
    ├── task6_regression_results.csv
    ├── task6_customer_segmentation.png
    ├── task6_segment_spending.png
    └── task6_actual_vs_predicted.png
```

## Results and Evaluation

The project generates customer segmentation results, sales analysis visualizations, and regression evaluation metrics.

The actual numerical results are available in the notebook and exported CSV files.

The regression model is a baseline experiment. Its performance should be interpreted using the actual evaluation metrics rather than assumed to be accurate.

## Key Learning Outcomes

Through this project, I practiced:

- Data cleaning and preprocessing with Pandas.
- Exploratory Data Analysis and visualization.
- Feature engineering.
- Customer-level data aggregation.
- Unsupervised machine learning using K-Means.
- Regression modeling using Random Forest.
- Model evaluation and interpretation.
- Communicating analytical findings through a project report.

## Future Improvements

- Implement RFM (Recency, Frequency, Monetary) analysis.
- Compare different customer clustering algorithms.
- Improve sales prediction using additional relevant features.
- Apply time-based validation for forecasting.
- Develop an interactive sales dashboard using Power BI.

## Project Deliverables

- Jupyter Notebook containing the complete analysis.
- Detailed Word project report.
- Customer segmentation results.
- Regression evaluation results.
- Data cleaning summary.
- Generated data visualization charts.

## Author

**Ayush Kumar**

GitHub: [ayushkumar789-eng](https://github.com/ayushkumar789-eng)

## Program

**YuvaIntern – Data Science Program**

**Task:** Week 6 – Integrative Capstone Project

---

If you find this project useful, feel free to explore the notebook and project outputs.

**Thank you for visiting!**
