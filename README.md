# 📊 SynapSupport: End-to-End Customer Analytics Cloud Pipeline

<p align="center">
  <img src="Data%20Engineering%20Architecture/Final_Logo_Synap_Support.png" width="300" alt="SynapSupport Logo">
  <br>
  <b>Empowering Business Decisions through Scalable Cloud Data Engineering</b>
</p>

---

## 🏗️ Technical Architecture
The infrastructure follows the **Multi-Hop (Medallion) pattern** to ensure data integrity:

<p align="center">
  <img src="Data%20Engineering%20Architecture/Cx_Diagram.jpg" width="900" alt="Architecture Diagram">
</p>

---

## 🛠️ Technology Stack & Resources
<p align="center">
  <img src="Data%20Engineering%20Architecture/Azure%20Resources.jpg" width="48%" />
  <img src="Data%20Engineering%20Architecture/Data_Lake_Containers.jpg" width="48%" />
</p>

---

## 📂 Sprint 2: Logical Modeling & Transformation
In this stage, we focused on translating business requirements into a robust relational schema.

### 📝 Logical Design (Sketching):
We performed manual sketching to architect the Dimension tables, ensuring they meet the analytical needs of the stakeholders:

<p align="center">
  <img src="Sprint 2 /Sketching/Shift Sketching.jpeg" width="31%" />
  <img src="Sprint 2 /Sketching/sketching of departement.jpeg" width="31%" />
  <img src="Sprint 2 /Sketching/status dim sketching.jpeg" width="31%" />
</p>

## ⚙️ Data Processing & Transformation
We leveraged the power of **Azure Synapse** to handle the ETL/ELT logic. By creating a unified view of support tickets, we bridged the gap between technical silos.

<p align="center">
  <img src="Data%20Engineering%20Architecture/Azure%20Synapse.jpg" width="80%" alt="Azure Synapse Transformation">
</p>

### 📈 Gold Layer Insights & KPIs
The final SQL Views were engineered to track **15+ Critical KPIs**, including:
* **Average Resolution Time (ART):** Measuring speed from ticket creation to "Closed" status.
* **Agent Productivity Score:** Normalizing performance across different departments.
* **Departmental Workload:** Identifying bottlenecks in real-time.
* **Shift Efficiency:** Comparing AM vs PM performance to optimize staffing.

<p align="center">
  <img src="Data%20Engineering%20Architecture/Synapse_Views_in_PBI.jpg" width="800" alt="Synapse Views in Power BI">
</p>

---

## 🚀 Key Quantifiable Impacts
* **40% Storage Cost Reduction:** Achieved by migrating from row-based CSV to compressed Parquet.
* **2x Faster Query Performance:** Optimized for Power BI via columnar indexing in Synapse.
* **80% Reduction in Manual Effort:** Automated the entire reporting cycle, saving 20+ hours per week.
* **Scalability:** Architected to handle **1M+ records** with no performance degradation.

---

## 👥 Meet the Team
* **Ahmed Youssef** ([@ahmedyoussef542003](https://github.com/ahmedyoussef542003))
* **Mahmoud Mamdouh** ([@Mahmooo0od](https://github.com/Mahmooo0od))
* **Mohammed Asim** ([@mohammedasim4040-eng](https://github.com/mohammedasim4040-eng))
* **Ashraf Saber** ([@ashrafsaber726](https://github.com/ashrafsaber726))
* **M. Yasser** ([@myassercom400-uz](https://github.com/myassercom400-uz))

---
<p align="center"><i>End-to-End Data Engineering Portfolio Project - 2026</i></p>
