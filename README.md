# Azure Data Engineering Project — E-Commerce Analytics (Bronze–Silver–Gold)
## Scalable ETL on Azure Databricks • Medallion Architecture • Analytics-Ready Data

![Azure](https://img.shields.io/badge/Azure-Databricks-blue)
![Data Engineering](https://img.shields.io/badge/Data%20Engineering-ETL%20Pipelines-green)
![Spark](https://img.shields.io/badge/Apache%20Spark-PySpark-orange)


---

**Author:** Tirumala Teja Yegineni  


---

## 📌 Overview

This project implements an **end-to-end Azure Data Engineering pipeline** for **E‑Commerce analytics** using **Apache Spark on Azure Databricks**, following the **Medallion (Bronze → Silver → Gold) architecture**.

It demonstrates how to ingest **large, semi-structured datasets**, clean and standardize them, and produce **business-ready analytical tables** suitable for BI and downstream ML.

---

## 🧱 Architecture (Medallion)

```
Raw CSV / Public Datasets
        ↓
Bronze Layer  (Raw ingestion)
        ↓
Silver Layer  (Cleaning & normalization)
        ↓
Gold Layer    (Business aggregations & KPIs)
```

---

## 📂 Repository Structure

```
ECommerce Data Analysis Azure Data Engineering/
│
├── Broze_Layer.ipynb        # Raw ingestion (Bronze)
├── Silver_Layer.ipynb       # Cleaning & normalization (Silver)
├── Gold Layer.ipynb         # Business KPIs & aggregates (Gold)
│
├── data/
│   ├── users.6M0xxK.2024.public.csv
│   ├── 6M-0K-99K.users.dataset.public.csv
│   ├── Buyers-repartition-by-country.csv
│   ├── Comparison-of-Sellers-by-Gender-and-Country.csv
│   ├── Countries-with-Top-Sellers-(Fashion-C2C).csv
│   ├── chunk-user-data.ipynb
│   └── chunk-data/
│       ├── chunk1.csv ... chunk10.csv
```

---

# 🧪 Pipeline Stages (Detailed)

---

## 1️⃣ Bronze Layer — Raw Data Ingestion

**Notebook:** `Broze_Layer.ipynb`

### Responsibilities
- Ingest raw CSV datasets into Spark
- Preserve original schema and values
- Handle large datasets via chunking

### Concepts Demonstrated
- Schema inference
- Distributed ingestion
- Raw data preservation


“Why do we keep a raw Bronze layer?”

---

## 2️⃣ Silver Layer — Cleaning & Normalization

**Notebook:** `Silver_Layer.ipynb`

### Responsibilities
- Data cleaning (nulls, types, duplicates)
- Column standardization
- Schema enforcement
- Data quality improvements

### Concepts Demonstrated
- Data cleansing at scale
- Spark transformations
- Preparing analytics-grade data

 
“What happens in the Silver layer?”

---

## 3️⃣ Gold Layer — Business Analytics

**Notebook:** `Gold Layer.ipynb`

### Responsibilities
- Business-level aggregations
- KPI computation
- Country-wise and gender-wise analysis
- Seller and buyer insights

### Outputs
- Analytics-ready tables
- BI-friendly datasets

 
“What kind of data belongs in the Gold layer?”

---

## 📊 Example Analytics Produced

- Buyer distribution by country  
- Seller comparison by gender & region  
- Top countries by seller activity  
- Large-scale user segmentation  

---

## 🧠 Key Skills Demonstrated

- Azure Databricks & Spark
- Medallion (Bronze–Silver–Gold) architecture
- Distributed ETL pipelines
- Data cleaning & normalization at scale
- Analytics-ready data modeling

---

## ⚙️ How to Run

### On Azure Databricks
1. Import notebooks into Databricks workspace  
2. Attach to a Spark cluster  
3. Run Bronze → Silver → Gold sequentially  

---

## 🧾  Points 

- Built an **Azure Databricks data engineering pipeline** for E‑Commerce analytics using **Apache Spark and PySpark**.  
- Implemented **Medallion architecture (Bronze, Silver, Gold)** to separate raw, clean, and business-ready data.  
- Processed **multi-million‑row datasets** using distributed Spark transformations.  
- Designed **Gold-layer KPIs and aggregations** to support analytics and BI reporting.  
- Demonstrated production-style **ETL design, scalability, and data quality practices**.

---

## 🧠 I Points

- “Bronze keeps raw data immutable.”
- “Silver enforces quality and schema.”
- “Gold is optimized for analytics and business queries.”
- “Spark enables scalable processing of millions of rows.”

---

## 👤 Author

**Tirumala Teja Yegineni**  
GitHub: https://github.com/TIRUMALA9999
