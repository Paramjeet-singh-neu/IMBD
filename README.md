# 🎬 IMDb Analytics & Data Warehouse Platform  

An end-to-end **Data Engineering + BI System** built to transform raw IMDb datasets into an analytics-ready lakehouse with dimensional modeling and interactive dashboards.

---

## 📌 Project Overview  

This project implements a **Bronze → Silver → Gold (Medallion) Architecture** to ingest, transform, and model IMDb data (~25M+ rows across 9 datasets) into a scalable analytics platform.

The system enables:
- Ratings trend analysis  
- Genre performance benchmarking  
- Regional release insights  
- Episode and season-level analytics  
- Self-serve executive dashboards  

The objective was to design a production-style analytics pipeline with proper data validation, modeling best practices, and version-controlled transformations.

---

## 🏗️ Architecture  

**Architecture Pattern:** Medallion Architecture (Lakehouse Design)

Raw Data (Bronze)  
        ↓  
Cleaned & Standardized Data (Silver)  
        ↓  
Dimensional Models / Fact & Dimension Tables (Gold)  
        ↓  
BI Dashboards (Power BI / Tableau)

---

## 🔹 Bronze Layer
- Raw IMDb datasets ingested as-is  
- Stored in cloud storage  
- Minimal transformation  
- Schema validation and profiling  

## 🔹 Silver Layer
- Data cleaning and normalization  
- Standardized schemas  
- Data quality checks (null handling, deduplication)  
- Data type enforcement  

## 🔹 Gold Layer
- Dimensional modeling (Star Schema)  
- Fact and dimension tables optimized for BI queries  
- Incremental transformations  
- Tested models (unique, not_null, relationships)

---

## 🗂️ Datasets Used  

The platform integrates 9 IMDb datasets including:

- Titles  
- Ratings  
- Episodes  
- Personnel  
- Genres  
- Regions  
- Languages  

**Total volume:** ~25M+ rows  

---

## 🧱 Data Model  

### Fact Tables
- `fact_titles`
- `fact_ratings`
- `fact_episodes`

### Dimension Tables
- `dim_titles`
- `dim_personnel`
- `dim_genres`
- `dim_regions`
- `dim_languages`

Modeling approach:
- Star schema  
- Surrogate keys  
- Proper foreign key relationships  
- Optimized for analytical queries  

---

## ⚙️ Tech Stack  

### Data Engineering
- Azure Data Factory (ADF)  
- Databricks  
- dbt (staging → marts)  
- Snowflake / Azure SQL  
- Git  

### Programming
- Python  
- SQL  

### BI & Analytics
- Power BI  
- Tableau  

---

## 🔎 Key Features  

- Scalable Lakehouse Architecture  
- Data Profiling and Validation Checks  
- Incremental Models with dbt  
- Reusable Macros  
- Relationship and Integrity Testing  
- Analytics-ready Star Schema  
- Interactive Dashboards  

---

## 📈 Business Questions Answered  

- Which genres consistently receive higher ratings?  
- How do ratings trend over time?  
- What regions produce the most high-rated titles?  
- How do episode ratings vary across seasons?  
- Which languages dominate high-performing content?  

---

## 📊 Dashboard Capabilities  

The BI layer enables:

- Genre-wise rating comparisons  
- Year-over-year rating trends  
- Regional content distribution  
- Top-rated titles analysis  
- Season performance visualization  

Designed for:
- Executives  
- Product analysts  
- Content strategists  
- Business stakeholders  

---

## 🚀 How to Run (High-Level)

1. Ingest raw IMDb datasets into Bronze layer  
2. Execute transformation pipelines (Databricks / dbt)  
3. Validate tests (unique, not_null, relationships)  
4. Load Gold tables into warehouse  
5. Connect Power BI / Tableau to Gold schema  
6. Refresh dashboards  

---

## 🧠 What This Project Demonstrates  

- Production-style data engineering  
- Dimensional modeling best practices  
- Data quality enforcement  
- End-to-end BI system design  
- Cloud-native analytics architecture  
- Stakeholder-ready reporting  

---


## 👨‍💻 Author  

**Paramjeet Singh**  
MS in Information Systems – Northeastern University  
Data Engineer | AI Engineer | Analytics Engineer  

📧 paramjeetsingh070@gmail.com  
🔗 LinkedIn: https://www.linkedin.com/in/paramjeet5ingh  
🌐 Portfolio: https://www.paramjeetsingh.me  
