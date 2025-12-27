# 🚀 Azure Batch Data Pipeline (Beginner Project)

## 📌 Project Overview
This project demonstrates a **beginner-friendly end-to-end Azure Data Engineering pipeline** that ingests raw sales data, processes it using best practices, and delivers business insights through **Power BI**.

The focus of this project is to understand **core data engineering concepts** such as batch ingestion, data cleaning, aggregation, and analytics — without overengineering.

---

## 🏗️ Architecture Overview

**Tools Used**
- Azure Data Factory (Data Ingestion)
- Azure Data Lake Storage Gen2 (Data Storage)
- Azure Databricks (Data Transformation)
- Power BI Desktop (Data Visualization)

---


## 🔄 Data Pipeline Flow

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/d5b5c30b-93e2-4de0-a146-e87265a5f01a" />


### 1️⃣ Data Ingestion (Azure Data Factory)
- Ingests sales data from CSV files
- Uses Copy Activity
- Manually triggered batch pipeline

### 2️⃣ Bronze Layer (Raw Data)
- Stores raw CSV data as received
- No transformations applied
- Append-only storage

### 3️⃣ Silver Layer (Clean Data)
- Removes duplicate records
- Handles null values
- Standardizes column names
- Stores cleaned data in Parquet format

### 4️⃣ Gold Layer (Analytics Data)
- Aggregates sales data by:
  - Date
  - Product
  - Region
- Creates analytics-ready datasets for reporting

### 5️⃣ Visualization (Power BI)
- Connects to Gold layer data
- Interactive dashboards showing:
  - Sales trends
  - Top products
  - Regional performance

---

## 🧱 Medallion Architecture Used

| Layer | Purpose |
|------|--------|
| Bronze | Raw, unprocessed data |
| Silver | Cleaned and validated data |
| Gold | Aggregated, business-ready data |

---

## 📊 Power BI Dashboard
The dashboard provides:
- Total sales over time
- Sales by product and region
- Filterable and interactive visuals

---

## 📁 Project Folder Structure

azure-batch-data-pipeline/
│
├── data/
│ ├── bronze/
│ ├── silver/
│ └── gold/
│
├── adf/
│ └── pipelines/
│
├── databricks/
│ └── notebooks/
│
├── powerbi/
│ └── dashboards/
│
├── diagrams/
│ └── architecture.png
│
└── README.md


---

## ⚙️ Key Concepts Demonstrated
- Batch Data Ingestion
- Azure Data Lake Gen2
- Medallion Architecture
- Data Cleaning & Deduplication
- Data Aggregation
- Star-schema-ready analytics
- Power BI Reporting

---

## 🚀 How to Run This Project
1. Upload CSV dataset to Azure Data Lake (Bronze)
2. Run Azure Data Factory pipeline
3. Execute Databricks notebooks:
   - Bronze → Silver
   - Silver → Gold
4. Open Power BI dashboard using Power BI Desktop

---

## 🎯 Learning Outcome
This project helped me understand:
- How real-world batch data pipelines work
- How to structure data using medallion architecture
- How data engineers support analytics teams

---

## 📌 Author
**Tanvi Nevagi  Siddhesh Gawde**  
Aspiring Data Engineer | Python | SQL | Azure | Power BI
