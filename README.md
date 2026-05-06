## Data Engineering Project (dbt Pipeline)

### Overview
This project is an end-to-end data pipeline built using **dbt (data build tool)**.  
It transforms raw data into clean, structured, and analytics-ready datasets using modular SQL models.

The main goal is to organize data workflows, apply transformations  and build reliable data marts for reporting and analysis.

---

### Tech Stack
- dbt (Data Build Tool)
- SQL
- python
- pyspark
- Databricks
- Git & GitHub
- Data Warehouse (PostgreSQL / BigQuery / Snowflake depending on setup)
- dbt Cloud 

---

### ⚙️ Data Pipeline Flow

1. **Bronze Layer**
   - Data is loaded into the warehouse from source systems

2. **Silver Layer**
   - Cleaning, renaming columns, fixing data types, handling nulls

3. **Gold Layer**
   - Applying business logic (joins, aggregations, calculations)

