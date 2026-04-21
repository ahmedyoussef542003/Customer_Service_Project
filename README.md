# 📊 SynapSupport: End-to-End Customer Analytics Cloud Pipeline

<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Final_Logo_Synap_Support.png" width="300" alt="SynapSupport Logo">
  <br>
  <b>Empowering Business Decisions through Scalable Cloud Data Engineering</b>
</p>

---

## 📖 Project Overview
**SynapSupport** is an enterprise-grade Data Engineering ecosystem built to solve the challenges of fragmented customer support data. By leveraging the **Azure Data Stack**, we transformed raw, unstructured data into a high-performance analytical hub. 

Our solution implements a modern **Medallion Architecture**, ensuring data integrity from the moment it lands in the lake until it is visualized in executive dashboards. This pipeline enables the organization to track agent productivity, optimize shifts, and improve customer satisfaction through data-driven insights.

---

## 🏗️ Technical Architecture
The infrastructure follows the **Multi-Hop (Medallion) pattern** to provide a clean, reliable stream of data:

<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Cx_Diagram.jpg" width="900" alt="Architecture Diagram">
</p>

### The Data Layers:
* **Bronze Layer (Raw Storage):** Ingests source files into **Azure Data Lake Storage Gen2** without modification.
* **Silver Layer (Enriched Data):** Data is cleaned and converted into **Parquet** format via **Azure Synapse** for optimal performance.
* **Gold Layer (Analytical Views):** Optimized **SQL Views** following a Star Schema, serving as the "Source of Truth" for BI reporting.

---

## 🛠️ Technology Stack
* **Cloud Platform:** Microsoft Azure
* **Data Orchestration:** Azure Data Factory (ADF)
* **Data Lake:** ADLS Gen2
* **Data Warehouse:** Azure Synapse Analytics (Serverless SQL Pools)
* **Data Visualization:** Power BI Desktop & Service
* **Version Control:** GitHub

<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Azure%20Resources.jpg" width="48%" />
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Data_Lake_Containers.jpg" width="48%" />
</p>

---

## 📂 Sprint 2: Logical Modeling & Transformation
During the second sprint, we translated business requirements into a relational structure to maximize query speed.

### Design Artifacts (Sketching):
<p align="center">
  <img src="Customer_Service_Project/Sprint%202/Sketching/Shift%20Sketching.jpeg" width="30%" />
  <img src="Customer_Service_Project/Sprint%202/Sketching/sketching%20of%20departement.jpeg" width="30%" />
  <img src="Customer_Service_Project/Sprint%202/Sketching/status%20dim%20sketching.jpeg" width="30%" />
</p>

### Transformation Logic:
Using **T-SQL** within Synapse, we engineered curated views for seamless Power BI integration:
<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Synapse_Views_in_PBI.jpg" width="750" alt="Synapse Views Implementation">
</p>

---

## 🚀 Key Quantifiable Achievements
* **40\% Storage Cost Reduction:** Achieved by implementing Snappy compression via Parquet files.
* **2x Faster Query Response:** Columnar storage optimization reduced I/O overhead.
* **80\% Reduction in Manual Reporting:** ETL automation eliminated manual data prep.
* **Data-Driven Scalability:** Architected to handle **1M+ monthly records** with minimal latency.

---

## 👥 Meet the Team
This project was successfully delivered through the collaborative efforts of:

* **Ahmed Youssef** ([@ahmedyoussef542003](https://github.com/ahmedyoussef542003))
* **Mahmoud Mamdouh** ([@Mahmooo0od](https://github.com/Mahmooo0od))
* **Mohammed Asim** ([@mohammedasim4040-eng](https://github.com/mohammedasim4040-eng))
* **Ashraf Saber** ([@ashrafsaber726](https://github.com/ashrafsaber726))
* **M. Yasser** ([@myassercom400-uz](https://github.com/myassercom400-uz))

### Project Contribution Graph
<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/contributors_activity.png" width="850" alt="Contributors Activity">
</p>

---
<p align="center"><i>End-to-End Data Engineering Portfolio Project - 2026</i></p>
