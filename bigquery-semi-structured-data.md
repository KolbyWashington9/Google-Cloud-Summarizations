BigQuery: Working with Semi-Structured Data (Arrays & Structs)
## Lab Overview

This lab explores how to handle semi-structured data in BigQuery, including arrays, structs, and nested/repeated fields.
You’ll ingest JSON, practice creating arrays and structs, and query nested datasets using functions like ARRAY_AGG() and UNNEST().
These skills are critical for working with real-world, denormalized datasets where performance and flexibility are key.


  ## Objectives

1.Load semi-structured JSON into BigQuery.

2.Create and query arrays.

3.Create and query structs.

4.Work with nested and repeated fields using UNNEST().

## Key Tasks

1.Dataset Creation

2.Created a dataset fruit_store to store lab tables.

3.Working with Arrays

4.Learned how arrays store multiple values in one field ([ ]).

5.Practiced creating arrays with ARRAY_AGG().

6.Explored ARRAY_LENGTH() and deduplication with ARRAY_AGG(DISTINCT ...).

7.Loading JSON with Repeated Fields

8.Ingested a JSON file (shopping_cart.json) into BigQuery.

9.Observed arrays stored as REPEATED fields.

10.Querying Existing Arrays

11.Used public Google Analytics datasets with native arrays.

12.Applied UNNEST() to flatten arrays into rows for analysis.

13.Working with Structs

14.Created and queried STRUCT fields (containers with multiple field types).

15.Noted how nested dot-notation works (struct.field).

16.Explored schemas containing RECORD types (STRUCTs).

17.Practice: Racing Dataset

18.Ingested race_results.json with nested structs and arrays.

19.Queried runners, lap splits, and total race times.

20.Used correlated CROSS JOIN + UNNEST() to unpack nested values.

## Key Learnings

1.Arrays in BigQuery are REPEATED fields — all values must share the same data type.

2.Structs (RECORD type) allow grouping of multiple fields into one container.

3.ARRAY_AGG() builds arrays from rows; UNNEST() flattens arrays back into rows.

4.Denormalization (ARRAYs + STRUCTs) can replace traditional JOINs, improving query performance.

5.Queries must account for different levels of granularity when working with nested data.

## Real-World Applications

1.E-commerce analytics: Track pageviews, product lists, and transactions in arrays.

2.Sports analytics: Store lap times, splits, and player stats in nested JSON.

3.Web analytics: Efficiently query complex, event-level Google Analytics data.

4.Data pipelines: Handle semi-structured logs and API responses without flattening at ingestion.

## Reflection

This lab was challenging but valuable for understanding nested and repeated fields in BigQuery.
The combination of STRUCT and ARRAY data types provides flexibility for complex data but requires careful use of UNNEST() to avoid errors.
I want to further practice optimizing queries with nested schemas and explore how denormalization impacts performance at scale.
