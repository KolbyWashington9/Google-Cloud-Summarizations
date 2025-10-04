BigQuery: Partitioned Tables for Cost & Performance Optimization

 Lab Overview

This lab demonstrates how to use partitioned tables in BigQuery to optimize query performance and reduce cost.
You’ll work with an ecommerce dataset (Google Merchandise Store Analytics) and NOAA weather data to:

1.Explore how non-partitioned queries scan large amounts of data.

2.Create date-partitioned tables.

3.Implement auto-expiring partitions for data compliance and storage efficiency.

 Objectives

1.Query non-partitioned datasets and observe cost implications.

2.Create date-partitioned BigQuery tables.

3.Improve performance by scanning only relevant partitions.

4.Use auto-expiring partitions for regulatory and cost management.

 Key Tasks

1.Create Dataset

2.Created an ecommerce dataset to store partitioned tables.

3.Query Non-Partitioned Data

4.Queried the all_sessions_raw table.

5.Even with filters (WHERE date = '20180708') and LIMIT 5, BigQuery still scanned 1.74 GB due to lack of partitions.

6.Create Date-Partitioned Table

7.Built ecommerce.partition_by_day table partitioned by date_formatted.

8.Verified metadata shows partitioning by Day.

9.Partition pruning reduced scanned data from 1.74 GB → 25 KB for relevant queries.

10.Auto-Expiring Partitioned Table

11.Used NOAA GSOD weather dataset (noaa_gsod.gsod*).

12.Created ecommerce.days_with_rain, partitioned by date, with:

partition_expiration_days = 60

13.Description = "weather stations with precipitation, partitioned by day"

 Validate Partition Expiration

14.Queried precipitation for Wakayama, Japan.

15.Used DATE_DIFF() to confirm oldest partitions were ≤ 60 days.

 Key Learnings

1.Partitioned tables allow BigQuery to skip irrelevant data, massively reducing scanned bytes and cost.

2.LIMIT does not reduce scan size — partitions do.

3.Partition expiration helps comply with data retention policies and control storage costs.

4.Public datasets often need to be reshaped into partitioned tables for efficient analysis.

 Real-World Applications

1.Web analytics: Focus queries only on recent visitor sessions.

2.Finance: Keep rolling 90-day transaction history with automatic expiration.

3.IoT & logs: Partition by event date to avoid scanning terabytes unnecessarily.

4.Compliance: Enforce data retention limits (e.g., GDPR) automatically.

 Reflection

This lab highlighted the cost-saving power of partitioning. Without partitions, even queries returning zero rows can scan gigabytes of data.
By partitioning and setting expiration, we improve both performance and governance.
I want to further experiment with clustering in BigQuery and how it can complement partitioning for even greater efficiency.
