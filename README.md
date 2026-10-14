# Superstore Sales & Profitability Analysis

## Executive Summary
This end-to-end data analysis project identifies loss-making sub-categories in the Superstore dataset, validates aggregation metrics via SQL queries, automates styled Excel reports using Python, and presents key business insights through an interactive Power BI dashboard.

## Key Findings
- **Loss-Making Sub-Categories:** Tables, Bookcases, and Supplies were identified as major drivers of negative profit across sub-categories.
- **Regional Performance:** The Central region exhibited lower overall profitability despite significant sales volume.
- **Sales vs Profit Discrepancy:** High sales volume does not guarantee high profitability, as observed in categories like Tables.

## Tech Stack
- **Python (pandas, openpyxl):** Exploratory Data Analysis (EDA), data cleaning, and automated Excel report generation.
- **SQL (SQLite):** Query verification and aggregation logic validation.
- **Excel:** Styled multi-sheet monthly report generation (`styled_loss_report.xlsx`).
- **Power BI:** Interactive BI dashboard development and data visualization.

## Data Pipeline Architecture
1. **EDA & Data Cleaning:** Processed raw Superstore data, extracted metrics, and exported cleaned data (`cleaned_superstore.csv`).
2. **SQL Verification:** Verified sales and profit aggregations using SQL queries.
3. **Excel Automation:** Built a Python script (`openpyxl`) to produce formatted, multi-sheet Excel reports (`styled_loss_report.xlsx`).
4. **Power BI Dashboarding:** Connected Power BI to `dashboard_data.xlsx` to build an interactive dashboard with key visuals (`Total Profit by Sub-Category`, `Total Profit by Region`, `Total Sales by Region`, and `Sales vs Profit by Sub-Category`).

## Project Structure
```text
├── data/
│   ├── cleaned_superstore.csv
│   ├── dashboard_data.xlsx
│   ├── loss_making_products.xlsx
│   └── styled_loss_report.xlsx
├── notebooks/
│   └── superstore_analysis.ipynb
├── dashboard/
│   ├── superstore_dashboard.pbix
│   └── dashboard_screenshot.png
└── README.md
