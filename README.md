Data Pipeline Project: Complete ETL and ELT Workflow
This repository contains two distinct data pipeline projects, showcasing both ELT and ETL workflows. Each project is tailored to different business requirements and utilizes a variety of data management tools to ensure reliable data ingestion, transformation, storage, and loading.

Project 1: ELT Pipeline
In the ELT pipeline, data is initially loaded to DWH storage as a backup and then transformed as needed based on specific business requirements.


Data Ingestion:
Raw data in CSV format is loaded into a flat file and then transferred to DWH_Storage as a backup.


Data Transformation:
Transformations are performed directly within the data warehouse, leveraging tools like Snowflake and dbt (Data Build Tool) to manipulate and prepare data for business intelligence (BI) analysis.


BI Layer / Production Layer:
Processed data is then stored in the BI/Production Layer, making it available for analytics and reporting.



Project 2: ETL Pipeline
In the ETL pipeline, a more structured transformation approach is followed, with data profiling and rigorous transformation steps before loading into the final storage layer.

Data Profiling:
The data is initially profiled to ensure accuracy and consistency.


Staging Area:
Data is staged in the DB_Stage area, where initial transformations are applied to prepare the data for processing.


Data Transformation:
Based on predefined logic, the data is transformed to create Master Data Management (MDM) tables, Business Intelligence (BI) tables, and Aggregated tables (e.g., sales by city).


Golden Layer:
Once transformed, the data is loaded into the Golden Layer for high-quality storage, enabling it to support further analysis and BI applications.
