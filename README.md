# AWS + Snowflake + dbt Data Pipeline

A data engineering project built around **AWS S3, Snowflake, and dbt**.

The goal is to build a simple end-to-end pipeline that takes raw data from S3, loads it into Snowflake, and transforms it into clean analytical models using dbt.

## Stack

* AWS S3
* Snowflake
* dbt
* Git & GitHub

## Architecture

```text
Raw Data
   ↓
AWS S3
   ↓
Snowflake
   ↓
  dbt
   ↓
Bronze → Silver → Gold
```

## Project Goals

* Load raw data from S3 into Snowflake
* Build Bronze, Silver, and Gold layers
* Create reusable dbt models and macros
* Handle incremental transformations
* Apply data quality checks
* Maintain the project using Git

## Build Steps

1. Set up the AWS S3 bucket and upload source data
2. Create the Snowflake database, schema, stages, and file formats
3. Load data from S3 into Snowflake
4. Initialize the dbt project
5. Build Bronze models
6. Build Silver transformations
7. Build Gold analytical models
8. Add tests, macros, and incremental logic
