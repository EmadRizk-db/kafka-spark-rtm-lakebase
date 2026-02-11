# kafka-spark-rtm-lakebase

## Overview

This repository contains two major notebooks demonstrating real-time data ingestion and processing using Kafka and Spark, with data landing in Lakehouse tables.

## Notebooks

- **1-create-and-save-test-data-to-kafka-read-topic**  
  Covers ingesting streaming data from Kafka topics into Spark DataFrames, including schema inference, parsing, and basic transformations.

- **2-read-kafka-store-to-lakebase-realtime**  
  Demonstrates ETL best practices for writing streaming data into Delta Lake tables, handling upserts, and optimizing for analytics.

## Usage

1. Clone this repository into your Databricks workspace.
2. Open and run the notebooks in order:
   - `01_create_and_save`
   - `02_read_kafka`
3. Follow the instructions in each notebook to configure Kafka endpoints and Delta Lake destinations.

## Requirements

- Databricks Runtime 17.3+ (or compatible)
- Access to a Kafka cluster
- Unity Catalog enabled workspace

