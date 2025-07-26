# 🏥 340B Data Integration & Analytics Pipeline – Microsoft Fabric

This project showcases a fully automated data engineering pipeline for processing 340B pharmacy data using **Microsoft Fabric**. It applies the **Medallion Architecture (Bronze → Silver → Gold)** and provides real-time Power BI dashboards for pharmacy leadership and compliance teams.

---

## ⚠️ Data Privacy Note

🧪 **All data in this project is synthetically generated using Python libraries (`faker`, `pandas`)**.  
There is **no real patient, provider, or claims data** used — making it safe for public use and fully reproducible.

---

## 🧰 Tools & Technologies

- **Microsoft Fabric**: Lakehouse, Pipelines, Dataflow Gen2
- **PySpark Notebooks**: Bronze layer ingestion
- **Dataflow Gen2**: Silver and Gold layer transformations
- **Power BI**: Dashboards and KPIs
- **Python**: Data simulation using `faker`, `pandas`

---

## 📊 Architecture Overview

1. OneLake (Monthly CSVs dropped)  
2. PySpark Notebook (Bronze Layer: Ingest raw files)  
3. Dataflow Gen2 (Silver Layer: Clean, Deduplicate, Join)  
4. Dataflow Gen2 (Gold Layer: Star Schema Fact/Dim Modeling)  
5. Power BI (Dashboards for analytics and reporting)

---

## 📁 Repository Structure

/
├── README.md                            → This file  
├── 340B_Fabric_Project_Asad_Patel.pdf  → Project documentation  
│
├── data/  
│   ├── sample_raw/                      → Synthetic CSV files  
│
├── notebooks/  
│   ├── bronze_ingestion.ipynb  
│   ├── bronze_notebook_code.png  
│   └── bronze_table_preview.png  
│
├── dataflows/  
│   ├── silver_dataflow_overview.png  
│   ├── gold_dataflow_star_schema.png  
│
├── dashboards/  
│   ├── eligibility_dashboard.png  
│   ├── prescriptions_dashboard.png  
│   ├── claims_revenue_dashboard.png  
│   ├── dispensing_kpis.png  
│   └── inventory_tracking_view.png  
│
├── pipeline_trigger/  
│   ├── pipeline_trigger_settings.png  
│   └── pipeline_flow_steps.png  
│
├── assets/  
│   ├── medallion_architecture_diagram.png  
│   └── data_pipeline_overview.png 

---

## 🧪 Synthetic Data Generation

Run the script below to generate the fake datasets used in this project:

```bash
cd data
python data_generator.py
```

This creates CSVs for:
- `eligibility.csv`
- `prescriptions.csv`
- `dispensing.csv`
- `claims.csv`
- `inventory.csv`
- `provider_roster.csv`

Each file contains hundreds of rows that simulate real-world hospital pharmacy data.

---

## 📈 Dashboards

This project delivers real-time, cross-domain analytics via Power BI:

- 🧬 340B Eligibility Monitoring  
- 💊 Prescription Oversight  
- 🚚 Dispensing Trends  
- 💰 Claims & Revenue Insights  
- 📦 Inventory Tracking  

Screenshots of each dashboard can be found in the `/dashboards` folder.

---

## ✅ Business Impact

- ⛔ Eliminated manual data entry  
- 🔄 Fully automated monthly processing pipeline  
- 📊 Real-time insights across pharmacy domains  
- ⚙️ Modular & scalable design for other hospital datasets

---

## 🔗 Connect With Me

- 📧 Email: asadpatel517@gmail.com  
- 💼 LinkedIn: [https://linkedin.com/in/asad--patel](https://linkedin.com/in/asad--patel)  
- 💻 GitHub: [https://github.com/apatel517](https://github.com/apatel517)

---

## 📄 View Full Project

👉 **[Click here to view the complete PDF](./340B_Fabric_Portfolio_AsadPatel_Final07.26.pdf)**
