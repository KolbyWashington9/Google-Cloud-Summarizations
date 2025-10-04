# BigQuery Bike & Weather Analysis – Google Cloud Training

##  Objective
Learn how to query and combine multiple public datasets in BigQuery to uncover real-world insights.  
Specifically, analyze bicycle rentals in New York City and weather patterns to determine correlations between rainy days and bike usage.

---

##  Tools & Services Used
- BigQuery  
- SQL Queries  
- Public Datasets (NYC Citibike, NOAA Weather Data)

---

##  Steps Performed
1. Explored the *New York City Citibike dataset* (`citibike_trips` and `citibike_stations`).  
   - Queried trip durations and most common rental routes.  
   - Calculated total distance traveled by each bike.  

2. Explored the *NOAA Weather dataset* (`ghcnd_2015`).  
   - Queried rainfall data for New York Central Park (Station: USW00094728).  

3. Joined bicycle rental and weather datasets.  
   - Compared average rentals on rainy vs. non-rainy days.  
   - Found a significant decrease in rentals during rainfall.  

---

##  Key Learnings
- BigQuery allows **serverless data analysis** with no need for clusters or index setup.  
- Public datasets can be combined seamlessly for insights.  
- SQL can answer **real-world correlation questions** (e.g., weather impact on transport).  
- Bike rentals in NYC dropped by ~47% on rainy days.  

---

##  Real-World Application
- *Urban planning & policy*: Helps cities understand how weather affects transportation usage.  
- *Data science pipelines*: Demonstrates how to cleanly join datasets from different sources for analysis.  
- *Business intelligence*: Retailers, insurers, or transport companies can use similar techniques to study demand fluctuations.  

---

##  Reflection
This lab showcased how quickly *ad-hoc queries* can reveal insights when working with large datasets on the cloud.  
I especially liked that I didn’t need to set up clusters or do heavy preprocessing — BigQuery handled it all.  
I want to further explore more *advanced SQL functions* and experiment with larger mashups of public datasets.  
