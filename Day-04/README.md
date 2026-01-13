# 📘 Day 4 – Delta Lake Introduction

## 🔍 Overview
Day 4 introduced **Delta Lake** and demonstrated how it enables **reliable, production-grade data pipelines** on top of Spark.

---

## 📚 What I Learned
- What **Delta Lake** is and why it is used  
- **ACID transactions** in big data systems  
- **Schema enforcement** and data quality protection  
- Differences between **Delta Lake** and **Parquet**

---

## 🛠️ What I Did
- Converted CSV data into **Delta format** using Databricks Volumes  
- Created **Delta tables** using both PySpark and SQL  
- Tested **schema enforcement** by attempting invalid writes  
- Handled **duplicate data** using deduplication logic

---

## 🧠 Delta Lake Concepts & Commands Practiced
```python
format("delta")       # Specify Delta format when writing
save()                # Save DataFrame as Delta table
saveAsTable()         # Save DataFrame as managed Delta table
dropDuplicates()      # Remove duplicate rows
CREATE TABLE USING DELTA  -- Create Delta table using SQL
