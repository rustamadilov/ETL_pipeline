# ETL pipeline
![Untitled design](https://github.com/user-attachments/assets/df9cfcc2-a14d-443e-902a-da9363ffe0e6)

## Overview

This ETL (Extract, Transform, Load) pipeline retrieves data from the SpaceX API, transforms the data into three separate tables, and loads these tables into a PostgreSQL database. The pipeline is orchestrated using Apache Airflow.

## Pipeline Components

- Extract: Fetches data from the SpaceX API and stores it using Airflow's XCom.
- Transform: Normalizes the JSON data into three separate pandas DataFrames and saves them as CSV files.
- Load: Creates tables in the PostgreSQL database and loads the transformed data from the CSV files into these tables.
