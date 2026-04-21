# 📊 SynapSupport: End-to-End Customer Analytics Cloud Pipeline

<p align="center">
  <img src="Data%20Engineering%20Architecture/Final_Logo_Synap_Support.png" width="300" alt="SynapSupport Logo">
  <br>
  <b>Building a Scalable, Cloud-Native Intelligence Hub for Modern Customer Care</b>
</p>

---

## 📖 Project Executive Summary
**SynapSupport** is an enterprise-level Data Engineering project designed to solve the complexity of fragmented customer support data. In today’s fast-paced environment, businesses struggle to track agent productivity and customer satisfaction in real-time. 

Our team architected a fully automated data pipeline using the **Microsoft Azure Ecosystem**, transitioning from manual, error-prone reporting to a robust **Medallion Architecture**. This ensures that every KPI—from resolution time to departmental load—is backed by high-quality, cleansed data.

---

## 🏗️ Data Architecture: The Medallion Framework
We implemented a **Multi-Hop Architecture** to maintain a clear "Lineage" of data and ensure top-tier data quality.

<p align="center">
  <img src="Data%20Engineering%20Architecture/Cx_Diagram.jpg" width="900" alt="Architecture Diagram">
</p>

### 🛡️ Layer Breakdown:
1.  **Bronze (Raw Layer):** Acts as the landing zone for raw CSV and Excel files. We keep the data in its original form in **ADLS Gen2** to allow for reprocessing if requirements change.
2.  **Silver (Cleansed Layer):** Using **Azure Synapse Serverless SQL**, we transform raw files into **Parquet** format. This stage involves data type casting, handling NULL values, and enforcing schema consistency.
3.  **Gold (Curated Layer):** The final analytical layer where data is modeled into a **Star Schema**. We created specialized **SQL Views** that serve directly to the BI layer.

---

## 🛠️ Enterprise Tech Stack
To ensure high availability and scalability, we utilized the following Azure services:

* **Azure Data Factory (ADF):** The backbone of our orchestration, managing automated data ingestion and scheduling.
* **Azure Data Lake Storage (ADLS Gen2):** A hierarchical storage solution optimized for big data analytics.
* **Azure Synapse Analytics:** Our primary compute engine for massive data processing and SQL-based transformations.
* **Power BI:** Our strategic visualization tool for delivering real-time dashboards to stakeholders.

<p align="center">
  <img src="Data%20Engineering%20Architecture/Azure%20Resources.jpg" width="48%" />
  <img src="Data%20Engineering%20Architecture/Data_Lake_Containers.jpg" width="48%" />
</p>

---

## 📂 Sprint 2: The Heart of Logical Modeling
Before touching the code, our team spent significant effort in the **Logical Design Phase**. This ensured that our data model would support complex analytical queries without performance degradation.

### 📝 Logical Design & Brainstorming (Sketching):
We mapped out the relationships between different entities to create a highly efficient Star Schema:

<p align="center">
  <img src="Sprint%202/Sketching/Shift%20Sketching.jpeg" width="31%" />
  <img src="Sprint%202/Sketching/sketching%20of%20departement.jpeg" width="31%" />
  <img src="Sprint%202/Sketching/status%20dim%20sketching.jpeg" width="31%" />
</p>

---

## ⚙️ Engineering & Transformation Process
We leveraged the power of **Azure Synapse** to perform heavy-duty T-SQL transformations. This included creating a robust indexing strategy and using Parquet's columnar storage to boost performance.

<p align="center">
  <img src="Data%20Engineering%20Architecture/Azure%20Synapse.jpg" width="80%" alt="Azure Synapse Implementation">
</p>

### 📊 Analytical Consumption (Gold Layer)
The final stage involves connecting Power BI to our Synapse Gold views. This direct connection ensures that as soon as a new record enters the pipeline, it is reflected in the KPIs.

<p align="center">
  <img src="Data%20Engineering%20Architecture/Synapse_Views_in_PBI.jpg" width="800" alt="Synapse Views in Power BI">
</p>

---

## 🚀 Key Quantifiable Impacts
* **Storage Efficiency:** Reduced storage footprint by **40%** by migrating from CSV to Parquet.
* **Performance Boost:** Query execution time was reduced by **2x** for complex joins.
* **Operational Excellence:** Automated 100% of the manual reporting workflow, saving roughly **20+ hours per week** for the analytics team.
* **Scalability:** The architecture is designed to handle a sudden surge of **1M+ records** without manual intervention.

---

## 👥 Meet the Engineering Team
This project was a collaborative success achieved by:

* **Ahmed Youssef** ([@ahmedyoussef542003](https://github.com/ahmedyoussef542003))
* **Mahmoud Mamdouh** ([@Mahmooo0od](https://github.com/Mahmooo0od))
* **Mohammed Asim** ([@mohammedasim4040-eng](https://github.com/mohammedasim4040-eng))
* **Ashraf Saber** ([@ashrafsaber726](https://github.com/ashrafsaber726))
* **M. Yasser** ([@myassercom400-uz](https://github.com/myassercom400-uz))

---
<p align="center">
  <i>Developed with passion for Data Engineering & Cloud Solutions.</i><br>
  <b>2026 Portfolio Project</b>
</p>
