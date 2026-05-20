# data-mining
contributors: 4 other peoples
# 📊 Customer Analytics & Churn Prediction Platform

## 🚀 Project Overview

This project focuses on building a complete **customer analytics and churn prediction pipeline** using modern **Data Engineering**, **Business Intelligence**, and **Machine Learning** practices.

The objective is to:

* centralize customer and behavioral data,
* process large-scale logs,
* predict churn risk,
* and deliver secure business dashboards through Power BI.

---

# 🏗️ Architecture

```text
Data Sources (CRM, Logs, Transactions)
        ↓
Raw Data Ingestion (JSON / Logs)
        ↓
Data Lake (immutable storage)
        ↓
ETL / Data Preparation
        ↓
Star Schema Data Warehouse
        ↓
Machine Learning (Churn Scoring)
        ↓
Power BI Dashboards (SSO + RLS)
```

---

# 📥 Data Sources

The platform integrates multiple data sources:

* CRM data
* Transactional systems
* Web/mobile logs
* Customer behavioral events

Raw data is ingested and archived in immutable format (JSON/logs) to ensure traceability and reproducibility.

---

# 🧹 Data Preparation

Main preparation tasks:

* data cleaning,
* normalization,
* duplicate handling,
* feature engineering,
* harmonization between CRM and production systems.

Special attention was given to:

* data granularity,
* customer ID consistency,
* multi-tenant data isolation.

---

# ⭐ Data Modeling

A **Star Schema** was implemented to optimize analytics performance in Power BI.

### Fact Table

* Sales
* Customer activity
* Churn indicators

### Dimension Tables

* Customers
* Products
* Dates
* Regions

Benefits:

* simplified joins,
* fast filtering,
* improved dashboard performance.

---

# 🤖 Machine Learning – Churn Prediction

A churn scoring model was developed using behavioral and transactional features such as:

* inactivity duration,
* session frequency,
* watch/purchase activity,
* weak signals extracted from logs.

The scoring pipeline was executed on an isolated Apache Spark cluster for scalable big data processing.

---

# 🔒 Security & Governance

The project includes:

* SSO authentication,
* Row-Level Security (RLS),
* client data isolation,
* tenant-based filtering.

This ensures secure and personalized access to dashboards.

---

# 📊 Business Intelligence

Dashboards were published through Power BI Service with:

* interactive KPI monitoring,
* churn analysis,
* customer segmentation,
* country-based filtering.

---

# 🛠️ Technologies Used

* SQL
* Python
* Apache Spark
* Power BI
* JSON / Logs
* ETL Pipelines
* Star Schema Modeling

---

# 🎯 Key Outcomes

* Centralized customer analytics platform
* Predictive churn scoring
* Scalable big data architecture
* Secure multi-client reporting
* Optimized BI performance
