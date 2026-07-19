# Week 6 - Spark Architecture and Performance

## Overview

This project was completed as part of the **Celebal Technologies Data Engineering Internship - Week 6 Assignment**.

The objective of this assignment is to understand Apache Spark architecture, DataFrame operations, schema handling, transformations, filtering, and performance optimization concepts. The project also demonstrates building a simple data processing pipeline using PySpark.

---

## Objectives

- Understand Spark Architecture (Driver, Cluster Manager, Executors)
- Learn Lazy Evaluation and DAG (Lineage Graph)
- Read CSV files with proper schema handling
- Perform DataFrame transformations and filtering
- Rename columns and cast data types
- Add derived columns
- Handle null values
- Compare CSV and Parquet file formats
- Build a simple Spark data pipeline
- Export processed data

---

## Dataset

**Dataset:** Ecommerce Sales Dataset

### Dataset Columns

- order_id
- customer_id
- product_id
- category
- price
- discount
- quantity
- payment_method
- order_date
- delivery_time_days
- region
- returned
- total_amount
- shipping_cost
- profit_margin
- customer_age
- customer_gender

---

## Technologies Used

- Python
- Apache Spark (PySpark)
- Pandas
- Jupyter Notebook
- VS Code

---

## Project Structure

```
week6-spark-architecture-performance/
│
├── data/
│   └── ecommerce_sales.csv
│
├── notebook/
│   └── spark_week6.ipynb
│
├── output/
│   └── csv_output.csv
│
├── README.md
└── .gitignore
```

---

## Tasks Performed

- Created Spark Session
- Loaded CSV dataset
- Applied schema inference
- Explored DataFrame
- Selected required columns
- Filtered records using conditions
- Renamed columns
- Cast data types
- Added new columns
- Handled null values
- Demonstrated Spark transformations and actions
- Built a data processing pipeline (Read → Transform → Filter)
- Exported processed dataset as CSV

---

## Spark Concepts Covered

- Spark Architecture
- Driver, Executors and Cluster Manager
- Lazy Evaluation
- DAG (Lineage Graph)
- Transformations
- Actions
- Wide Transformations
- Shuffle
- Predicate Pushdown
- CSV vs Parquet
- Schema Handling
- Data Pipeline

---

## Output

- Processed CSV dataset
- Spark notebook containing all assignment solutions
- Execution results and observations

---

## Note

The notebook includes the standard Spark command for exporting the processed DataFrame to Parquet:

```python
clean_df.write \
    .mode("overwrite") \
    .parquet("../output/parquet_output")
```

However, the Parquet export could not be completed in the local Windows environment due to Hadoop/WinUtils configuration limitations. All other Spark operations, including data loading, transformations, filtering, schema handling, and CSV export, were successfully executed.

In a properly configured Spark environment (Linux, Databricks, or Windows with Hadoop/WinUtils), the above command will generate the Parquet output without any changes.

---

## Learning Outcome

This assignment provided practical experience with Apache Spark DataFrames, Spark architecture, data transformations, filtering, schema handling, and performance optimization concepts used in data engineering workflows.


## Author

**MD SAHIL ANSARI**  
Data Engineering Intern  
Celebal Technologies