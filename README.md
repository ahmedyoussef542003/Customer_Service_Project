# 📊 SynapSupport: End-to-End Customer Analytics Cloud Pipeline

<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Final_Logo_Synap_Support.png" width="300" alt="SynapSupport Logo">
  <br>
  <b>Scalable Data Infrastructure for Intelligent Customer Support Insights</b>
</p>

---

## 📖 Executive Summary
**SynapSupport** is a comprehensive Data Engineering solution architected to automate the ingestion, transformation, and visualization of large-scale customer support datasets. Utilizing the **Azure Cloud Stack**, the project implements a **Medallion Architecture** to convert fragmented raw data into high-value, actionable business intelligence, empowering stakeholders to monitor agent performance and operational efficiency in real-time.

---

## 🏗️ Data Engineering Architecture
The pipeline is built on a multi-hop architecture designed for reliability and performance:

<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Cx_Diagram.jpg" width="850" alt="Data Pipeline Diagram">
</p>

### 🛡️ The Medallion Framework
1.  **Bronze (Raw):** Landing zone for original CSV/Excel files in **ADLS Gen2**, preserving the data in its native format.
2.  **Silver (Cleansed):** Data is processed via **Azure Synapse (Serverless SQL)**. Transformations include schema enforcement, handling nulls, and converting files to **Parquet** for optimized storage.
3.  **Gold (Curated):** Finalized **Star Schema** with Fact and Dimension views, optimized for analytical queries and BI consumption.

---

## 🛠️ Tech Stack & Azure Ecosystem
The project leverages enterprise-grade tools to ensure scalability:
* **Orchestration:** [Azure Data Factory (ADF)] for automated data movement.
* **Storage:** [Azure Data Lake Storage Gen2] with tiered containers (Bronze, Silver, Gold).
* **Compute/Warehouse:** [Azure Synapse Analytics] using Serverless SQL Pools.
* **Visualization:** [Power BI] for interactive reporting.
* **Collaboration:** [GitHub] for version control and CI/CD.

<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Azure%20Resources.jpg" width="48%" />
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Data_Lake_Containers.jpg" width="48%" />
</p>

---

## 📂 Sprint 2: Logical Modeling & Transformation
A core focus of this project was the transition from business requirements to technical logical modeling. We performed rigorous sketching to define optimized Dimension tables:

<p align="center">
  <img src="Customer_Service_Project/Sprint%202/Sketching/Shift%20Sketching.jpeg" width="30%" />
  <img src="Customer_Service_Project/Sprint%202/Sketching/sketching%20of%20departement.jpeg" width="30%" />
  <img src="Customer_Service_Project/Sprint%202/Sketching/status%20dim%20sketching.jpeg" width="30%" />
</p>

### Final Analytical Layers:
The transformation results in curated SQL Views within Synapse, allowing for seamless integration with Power BI:
<p align="center">
  <img src="Customer_Service_Project/Data%20Engineering%20Architecture/Synapse_Views_in_PBI.jpg" width="700" alt="Synapse Views in Power BI">
</p>

---

## 🚀 Key Quantifiable Achievements
* **40\% Storage Efficiency:** Achieved through Snappy compression in Parquet format.
* **2x Query Performance:** Realized by transitioning from row-based text files to columnar storage.
* **80\% Manual Effort Reduction:** Fully automated ETL pipelines replacing legacy manual reporting.
* **Real-time Tracking:** Supporting over **15+ KPIs** including Resolution Time, Agent Load, and Departmental Efficiency.

---

## 👥 Meet the Team (Authors)
This project was a collaborative effort by a dedicated team of Data Engineers:

* **Ahmed Youssef** ([@ahmedyoussef542003](https://github.com/ahmedyoussef542003)) - Lead Development & Optimization.
* **Mahmoud Mamdouh** ([@Mahmooo0od](https://github.com/Mahmooo0od)) - Architecture Design & Documentation.
* **Mohammed Asim** ([@mohammedasim4040-eng](https://github.com/mohammedasim4040-eng)) - Data Transformation.
* **Ashraf Saber** ([@ashrafsaber726](https://github.com/ashrafsaber726)) - BI Reporting & Quality Assurance.
* **M. Yasser** ([@myassercom400-uz](https://github.com/myassercom400-uz)) - Infrastructure Management.

<p align="center">
  <img src="https://raw.githubusercontent.com/YourUsername/SynapSupport/main/Documentation/contributors_activity.png" width="800" alt="Team Contribution Graph">
</p>

---
*Developed as part of an End-to-End Cloud Data Engineering Portfolio.*
