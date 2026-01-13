# Day 5 – Delta Lake Advanced 🚀

This day focused on **advanced Delta Lake features** that are essential for building **production-grade data engineering pipelines**. The objective was to move beyond basic ingestion and understand how Delta Lake handles **incremental updates, versioning, performance optimization, and storage cleanup**.

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
- Ensured ACID-safe updates

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

## 🧠 Delta Lake Concepts & Commands Practiced

```python
DeltaTable.forPath()          # Load an existing Delta table
merge()                       # Perform incremental upserts (MERGE INTO)
whenMatchedUpdate()           # Update records when match condition is met
whenNotMatchedInsert()        # Insert new records when no match is found

DESCRIBE HISTORY              # Inspect Delta table version history
option("versionAsOf")         # Time travel using table version
option("timestampAsOf")       # Time travel using timestamp

OPTIMIZE                      # Compact small files for better performance
ZORDER BY                     # Reorganize data layout for efficient filtering

VACUUM                        # Remove old, unreferenced data files
RETAIN HOURS                  # Define retention period for safe cleanup
