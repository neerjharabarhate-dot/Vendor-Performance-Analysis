# Vendor Performance Analysis

An end-to-end data analytics project focused on evaluating vendor performance, purchasing activity, sales contribution, profitability, and inventory efficiency using Python, SQLite, and Power BI.

## Project Overview

Vendor performance plays an important role in supply chain management. Understanding purchasing patterns, sales performance, profitability, and inventory movement helps businesses identify high-performing vendors, detect potential inefficiencies, and make better procurement decisions.

This project analyzes vendor-level data to evaluate purchasing and sales performance, examine profitability, and identify areas that may require further business attention.

## Business Objectives

- Evaluate vendor purchasing and sales performance.
- Identify vendors contributing the most to overall revenue.
- Analyze gross profit and profit margin across vendors.
- Examine inventory turnover and sales-to-purchase ratios.
- Identify vendors with negative gross profit or low stock turnover.
- Generate insights to support better procurement and inventory decisions.

## Tech Stack

- **Python:** Pandas, NumPy, Matplotlib, Seaborn
- **Database:** SQLite
- **Data Analysis:** Jupyter Notebook
- **Data Visualization:** Microsoft Power BI
- **Other Tools:** SQL, Excel

## Project Workflow

## 1. Dataset Overview

The project uses a comprehensive vendor performance dataset containing transactional and operational information related to purchases, sales, inventory, pricing, and vendor invoices.

The dataset consists of multiple interconnected files covering different aspects of vendor and inventory management.

**Dataset Files:**

| File | Description |
|---|---|
| `purchases.csv` | Vendor purchase transactions and purchasing details |
| `sales.csv` | Sales transactions and vendor-related sales information |
| `begin_inventory.csv` | Inventory levels at the beginning of the analysis period |
| `end_inventory.csv` | Inventory levels at the end of the analysis period |
| `purchase_prices.csv` | Product pricing information by vendor |
| `vendor_invoice.csv` | Vendor invoice and freight details |
| `vendor_sales_summary.csv` | Aggregated vendor-wise sales information |

**Dataset Details:**
- Format: CSV and SQLite database
- Dataset Version: 1
- Total Files: 8
- Main Focus: Vendor performance, purchasing, sales, and inventory analysis

The dataset supports analysis of vendor contribution, purchasing patterns, inventory movement, pricing, and overall supply chain performance.

**Dataset Licence:** CC0 – Public Domain.

### 2. Data Preparation & Vendor Summary

Combined purchasing and sales information to generate a vendor-level summary table.

The data preparation process included:
- Combining relevant vendor, purchase, and sales information.
- Cleaning and handling missing values.
- Calculating key performance metrics.
- Generating the `vendor_sales_summary` table.

The process and execution details were recorded in `get_vendor_summary.log`.

### 3. Exploratory Data Analysis (EDA)

Performed exploratory analysis using Python and SQLite to understand vendor performance and identify important patterns.

The analysis covered:
- Purchase and sales distribution.
- Vendor-level revenue contribution.
- Gross profit and profit margin.
- Inventory turnover.
- Sales-to-purchase ratio.
- Negative gross profit and low stock turnover.
- Correlation between purchasing and sales metrics.

### 4. Power BI Dashboard

Developed an interactive, single-page Power BI report to present vendor performance metrics and analytical findings through visual elements.

The report includes multiple visual configurations and embedded image assets to support its presentation and navigation.

## Key Analytical Findings

- **Dataset Size:** The vendor summary contains 12,490 records and 15 columns.
- **Negative Gross Profit:** 2,514 records showed negative gross profit.
- **Zero Sales:** 209 records had zero sales.
- **Low Stock Turnover:** 1,539 records had a stock turnover below 0.5.
- **Purchase and Sales Relationship:** Purchase quantity and sales quantity showed a strong positive correlation of approximately 0.999.
- **Revenue and Profit Relationship:** Total sales dollars and gross profit showed a strong positive correlation of approximately 0.972.

These findings highlight areas for further investigation, particularly vendors with negative gross profit, low inventory turnover, and limited sales activity.

## Project Deliverables

- Python Jupyter Notebook for exploratory data analysis.
- SQLite database ingestion and vendor summary pipeline.
- Execution logs for data ingestion and summary generation.
- Power BI dashboard for visual analysis.
- Project documentation.

## Repository Structure

```text
Vendor-Performance-Analysis/
│
├── README.md
│
├── Dashboard/
│   └── Vendor_Performance_Dashboard.pbix
│
├── Logs/
│   ├── ingestion_db.log
│   └── get_vendor_summary.log
│
├── Notebooks/
│   ├── Exploratory_Data_Analysis.ipynb
│   ├── Vendor_Analytics.ipynb
│   └── Vendor_Data_Analytics.ipynb
│
├── Scripts/
│   └── get_vendor_summary.py
│
├── Data/
│   └── vendor_sales_summary.csv
│
└── Screenshots/
    └── Vendor_Performance_Dashboard.png
```

## Conclusion

This project demonstrates an end-to-end approach to vendor performance analysis by combining data ingestion, preparation, exploratory analysis, and business intelligence reporting.

The analysis helps identify purchasing and sales patterns, evaluate vendor profitability, and highlight potential inventory inefficiencies. These insights can support more informed procurement and supply chain decisions.
