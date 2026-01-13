# 📘 Day 2 – Apache Spark Fundamentals

## 🔍 Overview
Day 2 focused on understanding how **Apache Spark** works internally and practicing core **DataFrame operations**.

---

## 📚 What I Learned
- Spark architecture: **Driver**, **Executors**, and **DAG**
- Difference between **DataFrames** and **RDDs**
- **Lazy evaluation** in Spark
- Databricks notebook **magic commands**: `%python`, `%sql`, `%fs`

---

## 🛠️ What I Did
- Uploaded an **e-commerce CSV dataset**
- Read data into a **Spark DataFrame**
- Performed **basic transformations** and **aggregations**
- Exported processed results

---

## 🧠 Spark Concepts & Commands Practiced
```python
spark.read.csv()       # Read CSV into DataFrame
select()               # Select columns
filter()               # Filter rows
groupBy()              # Group data
orderBy()              # Sort data
count()                # Count rows
write.csv()            # Write CSV output
write.parquet()        # Write Parquet output
