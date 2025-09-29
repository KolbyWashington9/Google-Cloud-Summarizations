# BigQuery Machine Learning (BigQuery ML)

## Objective

This lab focused on creating, training, evaluating, and using a machine learning model directly within BigQuery. The goal was to predict whether a visitor to the Google Merchandise Store would make a transaction, using SQL queries against a large Google Analytics dataset.

---

## Tools & Services Used

* BigQuery
* BigQuery ML (Logistic Regression)
* Google Analytics sample dataset
* Gemini Code Assist

---

## Steps Performed

1. *Explored the data**: Queried Google Analytics session data, prepared features such as operating system, device type, country, and pageviews, and saved the results as `training_data`.
2. *Created the model*: Used BigQuery ML to train a logistic regression model (`sample_model`) on the prepared dataset.
3. *Evaluated the model*: Applied `ML.EVALUATE` to measure the model’s accuracy and performance.
4. *Used the model*: Queried a new dataset (`july_data`) from a different time window, applied `ML.PREDICT` to generate predictions, and aggregated results to identify the top countries by predicted purchases.

---

## Key Learnings

* Machine learning models can be built and run directly in BigQuery without exporting data.
* Logistic regression is suitable for binary classification problems such as predicting transactions.
* `ML.EVALUATE` provides quick insights into a model’s performance.
* Debugging queries with Gemini Code Assist highlights common SQL mistakes, such as using unsupported aggregation functions.

---

## Real-World Application

BigQuery ML simplifies predictive analytics for analysts and engineers who already use SQL. Predictive models on customer behavior, churn, or conversions can be developed rapidly without additional infrastructure, making it practical for e-commerce businesses and marketing teams.

---

## Reflection

This lab reinforced how accessible machine learning becomes when integrated into BigQuery. I found the process of moving from raw analytics data to model creation straightforward, and the evaluation metrics provided helpful validation. Debugging with Gemini clarified syntax issues and showed the value of AI assistance in data workflows.
