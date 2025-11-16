# Stock Market Data Pipeline (Azure • Medallion Architecture • Power BI)

A fully scalable **End-to-End Stock Market Data Pipeline** built using the Azure ecosystem and aligned with the **Medallion Architecture (Bronze → Silver → Gold)**.
This project demonstrates real-world **cloud data engineering**, **PySpark transformations**, **lakehouse querying**, and **interactive BI reporting**.

---

## 🚀 Project Overview

This pipeline ingests raw stock market data, processes and enriches it using PySpark, creates analytics-ready datasets using Synapse Serverless SQL, and visualizes insights through a Power BI dashboard.

It is designed to show **modern data engineering best practices** on Azure.

---

## 🏗️ Architecture (Medallion Model)

<img width="762" height="488" alt="image" src="https://github.com/user-attachments/assets/ec9a0001-4d6e-4d2e-b10d-37945762dbcb" />


---

## 🧰 Tech Stack

* **Azure Data Factory (ADF)** – Pipeline orchestration
* **Azure Data Lake Storage Gen2 (ADLS)** – Bronze/Silver/Gold layers
* **Azure Databricks** – PySpark transformations
* **Azure Synapse Serverless SQL** – SQL querying and serving layer
* **Power BI** – Dashboard & insights
* **PySpark** – Data cleaning, enrichment, and aggregations

---

## 🔹 Pipeline Breakdown

### **1️⃣ Bronze Layer – Raw Ingestion**

* Parameterized pipelines in **Azure Data Factory**
* Lookup + ForEach to ingest multiple stock datasets
* Raw data stored as-is in ADLS (Bronze zone)

---

### **2️⃣ Silver Layer – Clean & Transform**

* Secure Databricks ↔ ADLS access using Service Principal
* PySpark transformations including:

  * `to_timestamp`, `year`, `month`
  * `concat_ws`, `groupBy`, window aggregations
* Optimized Parquet files stored in Silver zone

---

### **3️⃣ Gold Layer – Analytics Ready**

* Synapse OPENROWSET to query parquet data
* Created SQL Views + External Tables
* Gold zone data exported for BI consumption

---

## 📊 Power BI Dashboard

Included in this repo:

✔ Interactive visuals for trends, patterns & aggregates

✔ Stock-wise metrics and time-series insights

✔ Professional-level layout for storytelling


---

## 📌 Key Highlights

* End-to-end Azure data engineering workflow
* Scalable Medallion Architecture
* Real-world PySpark data processing
* Lakehouse + BI integration
* Production-style best practices

---

## 🤝 Connect with Me

If you’re a recruiter, engineer, or data enthusiast — I’d love to connect!
Let’s talk about cloud, data engineering, and scalable systems 🚀
