## Nashville Housing Market Analysis: Data Quality Remediation, Pricing Trends, and Market Segmentation

### Project Overview

This project analyzes Nashville housing transaction data using SQL and Python, with a strong emphasis on data quality validation, feature engineering, and market analysis.

The project was intentionally structured in two phases:

1. **Data Quality & Preprocessing**
   - validate raw data quality
   - investigate anomalies
   - clean inconsistent records
   - build analysis-ready dataset

2. **Market Analysis**
   - analyze pricing trends
   - evaluate regional differences
   - segment housing markets
   - identify valuation gaps

---

### Business Problem

Real estate transaction data often contains:

- duplicate records  
- inconsistent categorical values  
- missing fields  
- suspicious transactions  
- distorted pricing caused by bulk transfers  

Without resolving these issues first, downstream market analysis can produce misleading conclusions.

This project simulates how an analyst would clean messy transaction data before using it to support pricing strategy and market intelligence decisions.

---

### Dataset

**Source:** The dataset can be found at __[here](https://www.kaggle.com/tmthyjames/nashville-housing-data)__

The dataset includes:

- property transaction prices  
- property characteristics  
- land use categories  
- addresses  
- tax values  
- property age  
- ownership fields  

---

### Tech Stack

- SQL (SQLite)
- Python
- Pandas
- Jupyter Notebook

---

### SQL Environment

This project was implemented in **SQLite** for simplicity, portability, and reproducibility within a Jupyter Notebook workflow.

The analysis intentionally uses broadly transferable SQL concepts such as:

- CTEs  
- Window Functions  
- Views  
- Joins  
- Subqueries  
- Aggregations  

While SQLite was used for local development, the SQL logic can be easily adapted to production environments such as:

- PostgreSQL  
- SQL Server  
- Snowflake  
- BigQuery  

Stored procedures were intentionally not used because SQLite does not support them natively, and the project was designed to prioritize reproducible notebook-based analysis workflows.

---

### Project Structure

```bash
├── data/
│   ├── nashville_housing_data.xlsx
│   └── housing_final_cleaned.csv
│
├── notebooks/
│   ├── 01_data_quality_preprocessing_feature_engineering.ipynb
│   └── 02_housing_market_analysis_pricing_insights.ipynb
│
└── README.md
