Simple-ETL-Customer-Pipeline

Simple ETL Customer Pipeline: A mini data engineering project for cleaning, transforming, and preparing customer data. Includes handling missing values, duplicates, and basic data validation.
📌 Project: Customer Data Cleaning & Transformation
📖 Overview

This project demonstrates a simple Data Engineering pipeline for customer data.
The dataset is stored in a csv file (tab-separated) and contains customer information (ID, Name, Age, City).
The goal is to clean, transform, and prepare the data for further use (analysis, ML, or storage).
🔧 Steps in the Pipeline

 Extract Load customer data from .csv file using pandas.

Transform
        Convert column types:
            CustomerID → int64
            Name → string
            Age → Int64 (nullable integer)
            City → string
        Handle missing values (empty Age/City).
        Remove duplicates.
        Normalize text values (fix inconsistent city names, trim whitespaces).
        Validate data (Age range, unique IDs).

Load
        Export the cleaned dataset to CSV.
        Ready to be stored in a database or data warehouse.

        
📂 Files in Repository

customers.csv → raw data file.
    clean_customers.csv → cleaned dataset.
    data_pipeline.ipynb → Python script for ETL pipeline.
    README.md → project description.
