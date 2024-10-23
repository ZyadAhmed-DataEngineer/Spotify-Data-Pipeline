# Spotify Data Pipeline

## Overview
This project explores Spotify's data to measure artist popularity based on genre and follower count. An end-to-end data pipeline was built using AWS services, integrating data storage, transformation, and visualization. This pipeline is valuable for music labels, talent scouts, and analysts seeking insights into artist popularity trends.

## Project Workflow

### 1. Data Ingestion and Staging
- Imported CSV files containing Spotify data (artists, genres, follower counts) into an AWS S3 staging bucket.
- Set up two S3 buckets: one for staging and another for the data warehouse.

### 2. Data Transformation
- Utilized AWS Glue to build and execute the ETL pipeline.
- Converted data to the Parquet format for optimized storage and faster processing.
- Moved processed data to the S3 data warehouse.

### 3. Data Catalog and Crawler
- Employed AWS Glue Crawlers to create a schema and catalog the data in the data warehouse.
- Created a Glue Data Catalog to facilitate easy querying in AWS Athena.

### 4. Data Querying with Athena
- Queried the transformed data stored in S3 using Amazon Athena, enabling SQL-like queries directly on the data.

### 5. Data Visualization
- Used AWS QuickSight to visualize the data, generating insights into artist trends, genre-based popularity, and follower distribution.
- The visualizations provided clear insights into the most popular artists and genres on Spotify.

## Technologies Used
- **AWS S3:** Data storage (staging and warehouse).
- **AWS Glue:** ETL pipeline and data transformation.
- **AWS Glue Crawler:** Schema generation and data cataloging.
- **Amazon Athena:** SQL-based querying of data.
- **AWS QuickSight:** Interactive dashboards and data visualizations.

## Conclusion
This project provides a detailed look at how AWS services can be used to create a complete data engineering pipeline, from ingestion to visualization, while delivering meaningful insights into Spotify’s artist popularity trends.
