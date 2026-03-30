# Pyspark-sales-analysis
Pyspark - based data analysis project on sales dataset , including data cleaning , Transformations , aggregations and window functions
# 🍽️ Food Ordering Data Analysis using PySpark

## 📌 Objective

Analyze user ordering behavior and calculate cumulative order value using PySpark window functions.

## 🛠️ Tech Stack

* PySpark
* Google Colab
* Python

📊 Key Concepts Used

* Filtering
* Aggregations
* Window Functions (row_number, sum over window)

🔥 Sample Use Case

Calculated cumulative order value per day type using window functions.

💡 Key Code Snippet

python
window_spec = Window.partitionBy("day_type").orderBy("user_id")

df.withColumn(
    "Total_order_value",
    sum("order_value").over(window_spec)
)


🚀 Outcome

Learned real-world PySpark transformations
Built foundation for Data Engineering workflows

* Learned real-world PySpark transformations
* Built foundation for Data Engineering workflows
