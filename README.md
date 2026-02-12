# kafka-spark-rtm-lakebase

## Overview

This repository contains two major notebooks demonstrating real-time data ingestion and processing using Kafka and Spark, with data landing in Lakehouse tables.

## Notebooks

- **1-create-and-save-test-data-to-kafka-read-topic**  
  Covers ingesting streaming data to a Kafka topic with specified number of partitions and desired records per second rate.

- **2-read-kafka-store-to-lakebase-realtime**  
  Demonstrates RTM read from Kafka and writing to PostgesSQL best practices for data freshness and throughput control.

## Usage

1. Clone this repository into your Databricks workspace.
2. Open and run the notebooks in order:
   - `2-read-kafka-store-to-lakebase-realtime` in order to start the stream read path
   - `01-create-and-save-test-data-to-kafka-read-topic` in order to start writing to upstream Kafka topic which will be the downstream source
3. Follow the instructions in each notebook to configure Kafka endpoints and Delta Lake destinations.

## Requirements

- Databricks Runtime 17.3+ (or compatible)
- Access to a Kafka cluster
- Unity Catalog enabled workspace

