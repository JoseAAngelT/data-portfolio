🛒 Retail E-commerce Data Pipeline (Walmart Sales Analysis)

📌 Project Overview

This project builds an end-to-end data pipeline to analyze retail and e-commerce sales data from Walmart. The pipeline integrates multiple data sources, performs cleaning and transformation, and generates aggregated insights focused on weekly and monthly sales trends.

The goal is to simulate a real-world ETL process, including data extraction, transformation, aggregation, and validation.

🧠 Business Context

Walmart, the largest retail chain in the United States, has significantly expanded its e-commerce operations. By the end of 2022, online sales represented approximately $80 billion, accounting for 13% of total revenue.
Seasonal events such as Super Bowl, Labor Day, Thanksgiving, and Christmas have a strong impact on sales performance. This pipeline is designed to help analyze demand fluctuations around these holidays.

🎯 Project Objectives

The main objectives of this project are:

🔄 Build a modular ETL pipeline using Python functions
🧹 Clean and transform raw retail sales data
📊 Enrich data by combining multiple sources
📈 Generate monthly aggregated sales insights
💾 Export cleaned and aggregated datasets
✅ Validate pipeline outputs programmatically
🏗️ Pipeline Architecture

The pipeline is composed of four main stages:

1. Extract
- Load data from PostgreSQL table grocery_sales
- Load additional features from extra_data.parquet

2. Transform (transform() function)
- Merge datasets into a single DataFrame
- Handle missing numeric values
- Extract and create a Month column from Date
- Filter rows where Weekly_Sales > 10,000
- Remove unnecessary columns
- Output: clean_data

3. Aggregation (avg_weekly_sales_per_month() function)
- Select only relevant columns: Month, Weekly_Sales
- Group data by Month
- Compute average weekly sales per month
- Apply:
groupby()
agg()
reset_index()
round(2)
Output: agg_data

4. Load (load() function)
- Save processed datasets as CSV files:
clean_data.csv
agg_data.csv
- Files are saved without index

5. Validation (validation() function)
- Checks whether output CSV files exist in the working directory
- Ensures pipeline execution was successful
📊 Output Data
- Clean Dataset (clean_data)

Contains:

Store_ID
Month
Dept
IsHoliday
Weekly_Sales
CPI
Unemployment
Aggregated Dataset (agg_data)

Example structure:

Month	Weekly_Sales
1.0	33174.18
2.0	34333.33
...	...
🧰 Technologies Used
Python
Pandas
SQL (PostgreSQL)
Parquet files
Data manipulation & aggregation
🧪 Validation

To validate the pipeline output:

python

Run the validation() function to confirm that:

clean_data.csv exists
agg_data.csv exists
📁 Project Structure
.
├── notebook.ipynb
├── data/
│   └── extra_data.parquet
├── clean_data.csv
├── agg_data.csv
└── README.md
📌 Key Concepts Demonstrated

This project demonstrates core Data Engineering principles:

ETL pipeline design
Data integration from multiple sources
Data cleaning and feature engineering
Grouping and aggregation operations
Modular function-based architecture
Output validation and reproducibility
🚀 CV Summary Version

End-to-end retail data pipeline built in Python integrating SQL and parquet sources, performing data cleaning, transformation, aggregation, and validation to generate monthly sales insights for Walmart e-commerce analysis.