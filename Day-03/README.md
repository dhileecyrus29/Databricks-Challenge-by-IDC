# 📘 Day 3 – PySpark Transformations Deep Dive

## 🔍 Overview
Day 3 focused on **advanced PySpark transformations** used in real-world analytics and **feature engineering**.

---

## 📚 What I Learned
- Key differences between **PySpark** and **Pandas**
- Join types: **INNER**, **LEFT**, **RIGHT**, and **OUTER**
- **Window functions** for running totals and rankings
- Feature engineering using PySpark

---

## 🛠️ What I Did
- Loaded the full **e-commerce dataset**
- Performed **complex joins** using aggregated DataFrames
- Calculated **running totals** and **rankings** using window functions
- Created **derived features** for analytics and ML use cases

---

## 🧠 PySpark Concepts & Commands Practiced
```python
join()                        # Join DataFrames
Window.partitionBy().orderBy() # Define window for calculations
withColumn()                   # Create new or modify columns
when()                         # Conditional column values
sum()                          # Aggregate sum
count()                        # Count rows
row_number()                   # Assign row numbers in window
