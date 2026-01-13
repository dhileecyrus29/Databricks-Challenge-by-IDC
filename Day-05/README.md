# Day 5 – Delta Lake Advanced 🚀

This day focused on **advanced Delta Lake features** that are essential for building **production-grade data engineering pipelines**. The goal was to move beyond basic data ingestion and understand how Delta Lake manages **updates, versioning, performance, and storage cleanup**.

---

## 🔍 Topics Covered

- Incremental data processing using **MERGE (Upserts)**
- Querying historical data with **Time Travel** (version & timestamp)
- Improving query performance using **OPTIMIZE**
- Data layout optimization with **ZORDER**
- Storage management and cleanup using **VACUUM**

---

## 🛠️ Tasks Implemented

### 1. Incremental MERGE
- Simulated incoming ecommerce event data
- Performed upserts into an existing Delta table
- Handled schema differences using explicit column mapping

### 2. Time Travel
- Inspected Delta table version history
- Queried previous table states using:
  - Version numbers
  - Timestamps
- Validated historical snapshots before and after MERGE operations

### 3. Performance Optimization
- Compacted small files using OPTIMIZE
- Reorganized data using ZORDER on frequently filtered columns
- Improved query efficiency and data skipping

### 4. Data Cleanup
- Executed VACUUM with a safe retention period
- Understood retention policies and recovery limitations
- Learned the difference between file-level cleanup and row-level deletion

---

## 🧠 Key Learnings

- Delta Lake supports **ACID transactions** on data lakes
- MERGE enables scalable and safe incremental updates
- Time Travel is critical for debugging, auditing, and recovery
- OPTIMIZE and ZORDER significantly improve read performance
- VACUUM permanently removes unused files and must be used carefully

---

## 📁 Dataset

- Ecommerce events dataset
- Stored as a Delta table in Databricks
- Used to simulate real-world incremental updates and optimizations

---

## 🚀 Outcome

By the end of Day 5, the Delta table was:
- Incrementally updatable
- Fully versioned and auditable
- Performance optimized
- Storage-managed using best practices

---

## 🙏 Acknowledgements

Thanks to **Databricks**, **Codebasics**, and **Indian Data Club** for creating learning initiatives and challenges that promote hands-on, consistent learning.

---

## 🔗 Challenge

Part of the **Databricks 14-Day AI Challenge (DatabricksWithIDC)**

