# News-Data-Analysis

## Overview
The "News-Data-Analysis" project automates fetching news articles from the News API, storing them in Google Cloud Storage (GCS), and analyzing them using Snowflake. Apache Airflow orchestrates the entire workflow.

## Components
- Apache Airflow (GCP Composer)
- Google Cloud Storage (GCS)
- Snowflake
- News API

## Steps to Execute the Project

### Set Up GCP Environment
1. **Create a GCP Project**: Set up a new project in the Google Cloud Platform.
2. **Enable APIs**: Enable Google Cloud Storage and Google Composer APIs.
3. **Create GCS Bucket**: Create a GCS bucket (e.g., `snowflake_projects1`) for storing Parquet files.

### Configure Snowflake
1. **Create Snowflake Account**: Sign up for Snowflake and create a database.
2. **Set Up Storage Integration**: Link Snowflake with your GCS bucket to enable data transfer.

### Configure Airflow (GCP Composer)
1. **Set Up Airflow Environment**: Create an Airflow environment using GCP Composer.
2. **Deploy Airflow DAG**: Upload the DAG and Python scripts to the Airflow environment.

### Deploy the Python Script
1. **Create Fetch Script**: Write a Python script (`fetch_news.py`) to fetch data from the News API and upload it to GCS.

### Run the Data Pipeline
1. **Trigger the Airflow DAG**: Start the Airflow DAG to execute the data pipeline.
2. **Monitor Pipeline**: Ensure that tasks run successfully and data is correctly fetched, stored, and loaded.

### Analyze Data in Snowflake
1. **Query Data**: Use Snowflake to query and analyze the loaded data.

## Directory Structure
