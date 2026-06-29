# 🚀 End-to-End Uber Data Engineering Pipeline using Databricks & DBT Cloud

> An end-to-end modern data engineering project that ingests Uber trip data, transforms it using Databricks and dbt Cloud, and builds an analytics-ready data warehouse following the Medallion Architecture.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Databricks](https://img.shields.io/badge/Databricks-Lakehouse-red)
![dbt](https://img.shields.io/badge/dbt-Cloud-orange)
![Delta Lake](https://img.shields.io/badge/Delta-Lake-green)
![SQL](https://img.shields.io/badge/SQL-Analytics-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📌 Project Overview

This project demonstrates how to build a production-style data engineering pipeline using modern data stack tools.

The pipeline ingests raw Uber trip data into Databricks, cleans and transforms it through the Bronze, Silver, and Gold layers, applies modular SQL transformations using dbt Cloud, performs data quality testing, and creates analytics-ready fact and dimension tables for business intelligence.

The project follows industry best practices including:

- Medallion Architecture
- ELT Workflow
- Modular dbt Models
- Delta Lake Storage
- Data Quality Tests
- Incremental Data Processing
- Analytics-ready Star Schema

---

# 🏗 Architecture

```text
                 Raw Uber CSV
                       │
                       ▼
              Databricks File System
                       │
                Bronze Layer
             (Raw Delta Tables)
                       │
                       ▼
                Silver Layer
        (Cleaned & Standardized Data)
                       │
                       ▼
                 dbt Cloud Models
                       │
             Tests + Documentation
                       │
                       ▼
                 Gold Layer
     Fact & Dimension Tables
                       │
                       ▼
            Business Analytics
```

---

# ⚙ Tech Stack

| Category | Technology |
|-----------|------------|
| Language | Python |
| Data Processing | Apache Spark |
| Platform | Databricks |
| Data Storage | Delta Lake |
| Transformation | dbt Cloud |
| SQL Engine | Spark SQL |
| Version Control | Git & GitHub |
| Architecture | Medallion Architecture |
| Data Modeling | Star Schema |

---

# 📂 Project Structure

```text
End-to-End-Uber-Data-Engineering-Pipeline/

│
├── notebooks/
│   ├── Bronze Layer
│   ├── Silver Layer
│   └── Gold Layer
│
├── dbt/
│   ├── models/
│   ├── macros/
│   ├── snapshots/
│   ├── tests/
│   └── dbt_project.yml
│
├── datasets/
│
├── images/
│
└── README.md
```

---

# 📊 Medallion Architecture

## 🥉 Bronze Layer

Purpose:

- Store raw data
- Preserve original records
- Schema inference
- Delta table creation

Output:

```
bronze_uber_trips
```

---

## 🥈 Silver Layer

Purpose:

- Remove duplicates
- Handle null values
- Standardize data types
- Business rule validation
- Feature engineering

Output:

```
silver_uber_trips
```

---

## 🥇 Gold Layer

Purpose:

Create analytics-ready tables using Star Schema.

Includes:

- Fact Trips
- Date Dimension
- Location Dimension
- Passenger Dimension
- Payment Dimension

Optimized for reporting and BI dashboards.

---

# 🔄 Pipeline Workflow

```text
Uber Dataset
      │
      ▼
Databricks
      │
      ▼
Bronze Tables
      │
      ▼
Silver Tables
      │
      ▼
dbt Cloud
      │
      ├── Models
      ├── Tests
      ├── Documentation
      └── Lineage
      │
      ▼
Gold Tables
      │
      ▼
Analytics
```

---

# 📈 dbt Features Used

✅ Modular SQL Models

✅ Materializations

✅ Data Testing

- Unique Tests
- Not Null Tests
- Accepted Values

✅ Documentation

✅ Model Lineage

✅ Dependencies using `ref()`

---

# 📊 Data Model

### Fact Table

- Fact Trips

### Dimension Tables

- Date
- Pickup Location
- Dropoff Location
- Passenger
- Payment Type

The final warehouse follows a Star Schema suitable for reporting and dashboarding.

---

# 🚀 Key Features

- End-to-End ELT Pipeline
- Modern Data Stack
- Delta Lake Storage
- Medallion Architecture
- Modular dbt Models
- Data Quality Tests
- SQL Transformations
- Production-style Data Pipeline
- Analytics-ready Data Warehouse
- Version Controlled with GitHub

---

# 📌 Learning Outcomes

Through this project, I gained hands-on experience with:

- Databricks Lakehouse Platform
- Apache Spark
- Delta Lake
- dbt Cloud
- Data Modeling
- Star Schema Design
- Medallion Architecture
- SQL Transformations
- Data Testing
- Modern ELT Pipelines
- Git & GitHub

---

# 📷 Screenshots

Add screenshots of:

<img src="file:///C:/Users/Tanishq%20Saini/Pictures/Screenshots/Screenshot%202026-06-29%20183354.png
" alt="App Screenshot" width="500">
- Bronze Layer Tables
- Silver Layer Tables
- Gold Layer Tables
- dbt DAG
- dbt Documentation
- dbt Test Results

Example:

```
images/
│── architecture.png
│── dbt-lineage.png
│── bronze.png
│── silver.png
│── gold.png
```

---

# ▶ How to Run

### 1. Clone Repository

```bash
git clone https://github.com/tanishq826/End-to-End-Uber-Data-Engineering-Pipeline-using-Databricks-and-DBT-Cloud.git
```

### 2. Open Databricks

Import notebooks into your Databricks workspace.

### 3. Upload Dataset

Upload the Uber trip dataset to DBFS or Unity Catalog Volume.

### 4. Execute Bronze Pipeline

Create raw Delta tables.

### 5. Execute Silver Pipeline

Clean and transform data.

### 6. Connect dbt Cloud

- Configure Databricks connection
- Run models
- Execute tests
- Generate documentation

### 7. Query Gold Tables

Use Spark SQL or BI tools to analyze the transformed data.

---

# 📚 Concepts Demonstrated

- Data Engineering
- ETL / ELT
- Apache Spark
- Delta Lake
- Databricks
- dbt Cloud
- SQL
- Data Warehousing
- Star Schema
- Medallion Architecture
- Data Modeling
- Data Quality
- Analytics Engineering

---

# 🤝 Connect with Me

**Tanishq Saini**

- GitHub: https://github.com/tanishq826
- LinkedIn: *(Add your LinkedIn URL here)*

---

## ⭐ If you found this project helpful, consider giving it a star!
