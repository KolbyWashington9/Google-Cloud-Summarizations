BigQuery: Ingesting and Querying NYC Taxi Data
## Lab Overview

BigQuery is Google’s fully managed, serverless, low-cost analytics database that uses SQL and scales to analyze terabytes of data.
In this lab, you ingested NYC Taxi Trips datasets into BigQuery from multiple sources (CSV upload, Cloud Storage) and used DDL and SQL queries to explore and analyze the data.

## Objectives

1.Load datasets into BigQuery from different sources (local CSV, Cloud Storage).

2.Use CLI (bq load) and Console for ingestion.

3.Apply DDL (Data Definition Language) to create tables.

4.Query and analyze trip data for insights.

## Key Tasks

1.Create a Dataset

2.Created a new dataset nyctaxi to store taxi trip tables.

3.Ingest Data from CSV (Console)

4.Uploaded a subset of NYC Taxi 2018 trips.

5.Verified schema detection and row count (~10,018 rows).

6.Queried the top 5 most expensive trips → highest fare was $339.

7.Ingest Data from Cloud Storage (CLI)

8.Used bq load with --autodetect to append more data from Cloud Storage.

9.Verified that row count nearly doubled after ingestion.

10.Create Tables with DDL

11.Used CREATE TABLE ... AS SELECT to extract January trips into a new table january_trips.

12.Queried longest distance trip in January using ORDER BY trip_distance DESC.

## Key Learnings

1.BigQuery eliminates infrastructure management, enabling serverless analytics at scale.

2.Multiple ingestion options (upload, Cloud Storage, CLI).

3.DDL queries make it easy to transform datasets into focused subsets.

4.Ad-hoc SQL analysis can quickly reveal insights (e.g., longest trips, highest fares).

## Real-World Applications

1.Transportation analytics: Understanding seasonal demand, high-value trips, and route behaviors.

2.Data warehousing: Building pipelines for data ingestion from multiple sources.

3.Cost efficiency: Pay-as-you-go querying ensures analysis without upfront infrastructure costs.

## Reflection

This lab showed how flexible BigQuery is for loading, transforming, and querying large datasets.
I found the combination of console-based ingestion and CLI commands especially useful — it mirrors how engineers can work in real-world pipelines.
I’d like to further explore partitioned tables and query optimization in BigQuery for even larger datasets.
