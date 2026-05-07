## Medallion Data Engineering Pipeline using PySpark, Delta Lake & dbt

### Overview

This project demonstrates an end-to-end Data Engineering pipeline built using Databricks, PySpark, Delta Lake and dbt. The pipeline follows the Medallion Architecture approach with Bronze, Silver and Gold layers for scalable data ingestion, transformation and analytics.

The project processes multiple datasets including trips, customers, vehicles, locations and payments.

### Technologies Used

* Python
* PySpark
* Databricks
* Delta Lake
* dbt
* SQL
* YAML
* Jinja Templating
* Git

## Architecture

The project follows the Medallion Architecture:

### Bronze Layer

* Stores raw ingested data
* Handles initial data ingestion from source files
* Maintains raw data in Delta format

### Silver Layer

* Performs data cleaning and transformations
* Handles deduplication using window functions
* Implements CDC-based upsert logic using Delta Lake MERGE INTO
* Adds audit timestamps for tracking

### Gold Layer

* Builds analytical data models
* Implements star schema design
* Uses dbt snapshots for Slowly Changing Dimensions (SCD Type 2)
* Prepares data for downstream analytics and reporting

## Features

* Incremental data ingestion and processing
* Reusable PySpark transformation modules
* CDC-based upsert logic using Delta Lake
* Incremental dbt models
* Jinja templating for dynamic SQL generation
* Slowly Changing Dimensions (SCD Type 2)
* Star schema implementation
* Modular and scalable pipeline design

## Data Sources

The project processes the following datasets:

* Trips
* Customers
* Vehicles
* Locations
* Payments

## Key Implementations

### PySpark Transformations

Implemented reusable transformation modules for:

* Data deduplication
* Audit timestamp generation
* Incremental upsert operations
* Data quality handling

### dbt Models

Implemented dbt for:

* Incremental data models
* Snapshot management
* Schema configuration using YAML
* Jinja templating
* Gold layer modeling

### Slowly Changing Dimensions

Implemented SCD Type 2 using dbt snapshots to track historical changes in dimension tables.

### Learning Outcomes

Through this project, I gained hands-on experience in:

* Building Medallion Architecture pipelines
* Working with PySpark and Delta Lake
* Incremental data processing
* Data transformation and deduplication
* Using dbt for analytics engineering
* Implementing SCD Type 2
* Designing star schemas
* Managing data workflows in Databricks

### Future Improvements

Possible future enhancements:

* Add orchestration using Apache Airflow
* Integrate Kafka for real-time streaming
* Add automated data quality testing
* Deploy dashboards for analytics visualization
* Implement monitoring and alerting

## Conclusion

This project demonstrates a complete modern Data Engineering workflow using Databricks, PySpark, Delta Lake, and dbt. It showcases scalable data ingestion, transformation, modeling and analytics using a layered Medallion Architecture approach.
