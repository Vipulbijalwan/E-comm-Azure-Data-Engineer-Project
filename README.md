# 🛒 Ecomm Data Set – Azure Data Engineering Pipeline

## 📌 Overview
This project demonstrates a modern **data engineering pipeline** for processing the **E-commerce dataset** using the Azure ecosystem.  
The pipeline covers **data ingestion, transformation, enrichment, analytics, and visualization** using services like **Azure Data Factory, Azure Databricks, ADLS Gen2, Azure Synapse, and BI tools (Power BI/Tableau/Fabric).**

---

## ⚙️ Architecture

<img width="1535" height="864" alt="Screenshot 2025-08-26 115311" src="https://github.com/user-attachments/assets/1e739449-d932-4382-99b2-45d1a6c6439f" />

### 🔹 Steps in the Pipeline

1. **Data Sources**
   - Input data comes from:
     - **HTTP/GitHub (Ecomm dataset)**
     - **SQL Tables**

2. **Data Ingestion – Azure Data Factory**
   - Orchestrates data ingestion from GitHub/SQL.
   - Stores raw data in **Azure Data Lake Storage Gen2 (ADLS Gen2)**.

3. **Raw Data Storage – ADLS Gen2**
   - Acts as the **data lake (raw zone)**.

4. **Data Transformation – Azure Databricks**
   - Performs data cleaning, transformation, and enrichment.
   - Joins with **MongoDB** tables for additional enrichment.
   - Writes **processed data** back into **ADLS Gen2**.

5. **Analytics Layer – Azure Synapse**
   - Consumes transformed data for SQL-based queries and reporting.

6. **Visualization Layer**
   - Business insights are created using:
     - **Power BI**
     - **Tableau**
     - **Microsoft Fabric**

---

## 🛠️ Tech Stack

- **Azure Data Factory (ADF)** → Data ingestion & orchestration
- **Azure Data Lake Storage Gen2 (ADLS Gen2)** → Raw & processed data storage
- **Azure Databricks** → Data transformation & enrichment
- **MongoDB** → Enrichment data source
- **Azure Synapse Analytics** → Analytics & SQL queries
- **Visualization** → Power BI, Tableau, Fabric

---

## 🚀 Workflow

1. Ingest **Ecomm dataset** → **ADLS Gen2 (Raw Zone)** using **ADF**.
2. Transform raw data in **Azure Databricks**:
   - Cleaning
   - Aggregation
   - Enrichment (via MongoDB)
3. Store transformed data in **ADLS Gen2 (Processed Zone)**.
4. Load processed data into **Azure Synapse** for queries.
5. Build dashboards with **Power BI/Tableau/Fabric**.

---

## 📂 Project Structure

