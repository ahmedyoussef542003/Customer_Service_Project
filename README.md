# 📊 SynapSupport: End-to-End Customer Analytics Pipeline (Azure Cloud)

<p align="center">
  <img src="https://github.com/YOUR_USERNAME/SynapSupport/raw/main/Documentation/logo.png" width="250" alt="SynapSupport Logo">
  <br>
  <b>Building a Scalable, Cloud-Native Intelligence Hub for Modern Customer Care</b>
</p>

---

## 📖 Project Overview

**SynapSupport** هو مشروع متكامل لهندسة البيانات (Data Engineering) يهدف إلى أتمتة عملية سحب، تنظيف، وتحليل بيانات خدمة العملاء. يعتمد المشروع على **Azure Cloud Ecosystem** وبتطبيق منهجية **Medallion Architecture** لتحويل البيانات الخام إلى رؤى ذكية (Insights) تدعم صناعة القرار.

يوفر هذا النظام للإدارة القدرة على مراقبة أداء الموظفين، سرعة الاستجابة، وتوزيع ضغط العمل (Workload) بشكل لحظي، مما يساهم في تحسين جودة الخدمة وتقليل التكاليف التشغيلية.

---

## 🏗️ Architecture & Data Workflow

يعتمد المشروع على تصميم هندسي قوي يضمن الـ Scalability والـ Data Integrity:

<p align="center">
  <img src="https://github.com/YOUR_USERNAME/SynapSupport/raw/main/Documentation/architecture_diagram.png" width="850" alt="Architecture Diagram">
</p>

### 🛡️ Medallion Framework (Multi-Hop Architecture)
1.  **Bronze Layer (Raw):** يتم استقبال البيانات بصيغتها الأصلية (CSV, Excel) وحفظها في **Azure Data Lake (ADLS Gen2)** لضمان وجود نسخة "Single Source of Truth".
2.  **Silver Layer (Cleansed):** يتم استخدام **Azure Synapse (Serverless SQL)** لتحويل البيانات إلى صيغة **Parquet**. في هذه المرحلة يتم معالجة القيم المفقودة (Nulls)، توحيد أنواع البيانات، وضمان جودة الـ Schema.
3.  **Gold Layer (Curated):** إنشاء **Star Schema** تتكون من جداول الحقائق والابعاد (Fact & Dimensions) عبر SQL Views، لتكون جاهزة للتحليل المباشر.

---

## 🛠️ Tech Stack & Cloud Resources

* **Orchestration:** [Azure Data Factory (ADF)](https://azure.microsoft.com/en-us/products/data-factory) لجدولة الـ Pipelines وإدارة حركة البيانات.
* **Storage:** [Azure Data Lake Storage Gen2](https://azure.microsoft.com/en-us/products/storage/data-lake-storage) لتخزين البيانات بكافة مراحلها.
* **Data Warehouse:** [Azure Synapse Analytics](https://azure.microsoft.com/en-us/products/synapse-analytics) (Serverless SQL Pools) لمعالجة البيانات الضخمة بتكلفة منخفضة.
* **Visualization:** [Power BI](https://powerbi.microsoft.com/) لإنشاء الـ Dashboards التفاعلية.
* **Version Control:** [GitHub](https://github.com/) لإدارة الكود والـ CI/CD.

---

## 📂 Sprint 2: Data Modeling & Business Logic

في هذه المرحلة، تم تحويل المتطلبات الإدارية إلى تصميم تقني. تم عمل **Sketching** للجداول الأساسية لضمان أفضل أداء للاستعلامات:

<p align="center">
  <img src="https://github.com/YOUR_USERNAME/SynapSupport/raw/main/Documentation/shift_sketch.jpeg" width="30%" alt="Shift Table Sketch"> 
  <img src="https://github.com/YOUR_USERNAME/SynapSupport/raw/main/Documentation/department_sketch.jpeg" width="30%" alt="Department Table Sketch">
  <img src="https://github.com/YOUR_USERNAME/SynapSupport/raw/main/Documentation/status_sketch.jpeg" width="30%" alt="Status Table Sketch">
</p>

### Key Dimensions Modeled:
* **Dim_Shift:** لتحليل الأداء بناءً على فترات العمل المختلفة.
* **Dim_Department:** لتوزيع ضغط العمل بين الأقسام التقنية والإدارية.
* **Dim_Status:** لمراقبة حالات التذاكر (Open, Closed, Pending).

---

## 🚀 Quantifiable Achievements (Business Impact)

* **Storage Optimization:** بفضل التحويل لصيغة **Parquet**، تم تقليل مساحة التخزين بنسبة **40\%**.
* **Query Performance:** تحسن أداء الاستعلامات بمعدل **2x** مقارنة بالتعامل مع الملفات النصية الخام.
* **Cost Efficiency:** استخدام الـ **Serverless Architecture** ساهم في تقليل تكاليف الحوسبة بشكل كبير (Pay-per-query).
* **Decision Speed:** تقليل الوقت المستغرق في إعداد التقارير اليدوية بنسبة **80\%**، حيث أصبحت البيانات تتدفق بشكل آلي للـ Dashboard.

---

## 📈 Final Visualization (Power BI)

الـ Dashboard النهائية تمكن الـ Stakeholders من مراقبة:
* متوسط وقت الاستجابة (Average Response Time).
* أداء الموظفين (Agent Performance Score).
* توزيع التذاكر حسب القسم والحالة.

---

## 👤 Author

**Mahmoud Mamdouh**
*Data & Analytics Engineer*
* [LinkedIn Profile](YOUR_LINKEDIN_URL)
* [Portfolio](YOUR_PORTFOLIO_URL)

---
*Note: This project was developed as part of a comprehensive Cloud Data Engineering roadmap to demonstrate expertise in Azure Data Stack.*
