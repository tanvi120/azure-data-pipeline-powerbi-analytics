# 🚀 Azure End-to-End Data Engineering Project (Amazon Prime Analytics)

## 📌 Project Overview
This project demonstrates an **end-to-end Azure Data Engineering pipeline** that ingests raw data from an HTTP source, processes it using Azure Databricks, organizes it using **Medallion Architecture**, and delivers insights through **Power BI dashboards**.

The goal of this project is to understand and implement **core data engineering concepts** using Azure services in a simple, beginner-friendly manner.

---

## 🏗️ Architecture Overview

### Technologies Used
- **Azure Data Factory** – Data ingestion from HTTP source
- **Azure Data Lake Storage Gen2** – Data storage (Bronze, Silver, Gold)
- **Azure Databricks** – Data cleaning and transformations using PySpark
- **Power BI Desktop** – Data visualization and reporting

---

## 🔄 Data Pipeline Flow

### 1️⃣ Data Ingestion (Azure Data Factory)
- Data is ingested from an HTTP endpoint
- Uses **Copy Activity**
- No transformations during ingestion
- Raw data is stored in Azure Data Lake

---

### 2️⃣ Bronze Layer (Raw Data)
- Stores raw CSV data exactly as received
- Append-only storage
- Acts as a backup and source of truth

---

### 3️⃣ Data Transformation (Azure Databricks)
Using PySpark, the following operations are performed:
- Schema standardization
- Handling null values
- Data type corrections
- Basic data cleaning

---

### 4️⃣ Silver Layer (Clean Data)
- Cleaned and structured data
- Stored in optimized Parquet format
- Ready for analytical processing

---

### 5️⃣ Gold Layer (Business Data)
- Aggregated and analytics-ready data
- Optimized for reporting and visualization
- Examples:
  - Movies and TV shows by year
  - Content distribution by country
  - Genre-wise analysis

---

### 6️⃣ Visualization (Power BI)
- Power BI connects to Gold layer data
- Interactive dashboards created to analyze:
  - Content trends
  - Release patterns
  - Country-wise distribution

---

## 🧱 Medallion Architecture Used

| Layer | Description |
|------|------------|
| Bronze | Raw, unprocessed data |
| Silver | Cleaned and structured data |
| Gold | Aggregated, business-ready data |

---

## 📁 Project Structure

<img width="247" height="609" alt="image" src="https://github.com/user-attachments/assets/da51cfcd-390b-4f79-b131-1d63f759ed4a" />


---

## ⚙️ Key Concepts Demonstrated
- ETL Pipeline Design
- Azure Data Factory Copy Activity
- Azure Data Lake Storage Gen2
- Azure Databricks with PySpark
- Medallion Architecture (Bronze / Silver / Gold)
- Batch Data Processing
- Power BI Data Visualization

---

## 🚀 How to Run This Project
1. Ingest data using Azure Data Factory
2. Store raw data in Bronze layer
3. Run Databricks notebooks to generate Silver and Gold layers
4. Connect Power BI to Gold layer data
5. Build dashboards and insights

---

## 🎯 Learning Outcome
Through this project, I gained hands-on experience in:
- Designing Azure-based data pipelines
- Processing data using PySpark
- Organizing data for analytics
- Building BI dashboards using Power BI

---

## 📌 Dataset Source
Amazon Prime Movies and TV Shows Dataset  
https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows

---

## 👤 Author
**Tanvi Nevagi Siddhesh Gawde*  
Aspiring Data Engineer | Python | SQL | Azure | Power BI

