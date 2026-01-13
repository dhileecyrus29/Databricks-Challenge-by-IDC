# Day 0 – Setup & Data Loading (Prerequisites) ⚙️📥

Day 0 focuses on setting up the **Databricks environment** and performing **initial data loading**, which serves as the foundation for all subsequent days in the Databricks 14-Day AI Challenge. This step ensures the workspace, storage, and datasets are ready for advanced data engineering and analytics tasks.

---

## 🎯 Objective

- Prepare the Databricks workspace for the challenge
- Load raw data into Databricks
- Validate schema and data integrity
- Establish a baseline dataset for future transformations

---

## 🔍 Topics Covered

- Databricks workspace and notebook setup
- Reading external datasets into Spark
- Basic DataFrame inspection and validation
- Writing data to storage for downstream use

---

## 🛠️ Tasks Implemented

### 1. Environment Setup
- Verified Spark session availability
- Configured notebook and workspace settings
- Ensured required libraries and runtime were accessible

### 2. Data Loading
- Loaded the ecommerce dataset into Spark DataFrames
- Used schema inference and headers where applicable
- Verified successful ingestion using basic DataFrame actions

### 3. Data Validation
- Checked row counts and column names
- Inspected data types and schema
- Performed basic sanity checks to confirm data consistency

### 4. Data Persistence
- Stored the loaded data in Databricks storage
- Prepared the dataset for conversion to Delta format in later days

---

## 🧠 Spark & Data Engineering Concepts Practiced

```python
spark.read.csv()          # Read CSV files into Spark DataFrames
option("header", "true")  # Use first row as column names
option("inferSchema")     # Automatically infer data types

printSchema()             # Inspect DataFrame schema
show()                    # Preview data
count()                   # Validate record counts

write.format()            # Specify output data format
save()                    # Persist data to storage
