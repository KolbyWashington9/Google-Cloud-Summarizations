Cloud SQL: Importing and Analyzing NYC Taxi Trips
## Lab Overview

In this lab, you will learn how to import CSV data into Cloud SQL and perform basic data analysis using SQL queries.
The dataset is provided by the NYC Taxi & Limousine Commission, containing detailed trip records such as pickup/drop-off times, locations, fares, passenger counts, and payment types.

This dataset is widely used for data engineering and data science demonstrations.

## Objectives

1.Create a Cloud SQL instance and database

2.Import CSV data into a Cloud SQL table

3.Verify data integrity through queries

4.Run basic analytics on taxi trip data

 ## Key Tasks

1.Prepare the environment

2.Configure environment variables for project, region, and storage bucket

3.Activate Cloud Shell

4.Create Cloud SQL Instance

5.Provision a SQL instance with gcloud sql

6.Set root password and whitelist Cloud Shell for access

7.Create bts database and trips table schema

8.Import Taxi Trips Data

9.Copy sample CSVs (~20,000 rows) from Cloud Storage

10.Load data into trips table using LOAD DATA LOCAL INFILE

11.Check Data Integrity

12.Verify unique pickup locations

13.Inspect trip distances (0-mile trips detected)

14.Find negative fare values

15.Analyze payment types distribution

 Key Learnings

1.Cloud SQL Integration: Seamlessly import structured data for analysis.

2.Data Integrity Checks: Essential step in validating pipelines (detecting 0-distance trips, negative fares).

3.Real-World Relevance: Taxi trip datasets mimic real data engineering scenarios where cleaning and validation are critical.

## Real-World Applications

1.Fraud detection (e.g., suspicious zero-distance or negative-fare trips)

2.Transportation analytics (trip demand, payment methods, passenger trends)

3.Data pipelines for business intelligence and machine learning models

## Reflection

This lab demonstrates the process of moving raw CSV data into Cloud SQL and ensuring its integrity before downstream use.
By applying validation queries, data engineers can uncover anomalies and prepare the dataset for meaningful analysis and reporting.
