🛒 Ecomm Data Set – Azure Data Engineering Pipeline
📌 Overview

This project demonstrates a modern data engineering pipeline built on the E-commerce dataset using the Azure ecosystem.
The pipeline ingests raw data, stores it in a data lake, processes it with Databricks, enriches it with MongoDB, and finally makes it available for analytics and visualization through Synapse and BI tools.

⚙️ Architecture

🔹 Steps in the Pipeline

Data Sources

Input data comes from:

HTTP/GitHub (Ecomm dataset)

SQL Tables

Data Ingestion (Azure Data Factory)

Azure Data Factory orchestrates ingestion from multiple sources.

Raw data is landed into Azure Data Lake Storage Gen2 (ADLS Gen2).

Raw Data Storage (ADLS Gen2)

Stores the raw e-commerce dataset for further processing.

Data Transformation (Azure Databricks)

Raw data is cleaned, transformed, and enriched inside Databricks.

External MongoDB tables are used for additional enrichment.

Transformed data is saved back into ADLS Gen2.

Analytics Layer (Azure Synapse)

Transformed data is consumed in Azure Synapse Analytics for querying and reporting.

Visualization Layer

Business insights and dashboards are created using:

Power BI

Tableau

Microsoft Fabric

🛠️ Tech Stack

Azure Data Factory (ADF) → Data ingestion

Azure Data Lake Storage Gen2 (ADLS Gen2) → Data lake storage

Azure Databricks → Data cleaning & transformation

MongoDB → Enrichment data source

Azure Synapse Analytics → Query and analytics

Visualization → Power BI, Tableau, Fabric

🚀 Workflow

Ingest Ecomm dataset (from GitHub/SQL) → ADLS Gen2 (raw zone).

Transform raw data in Databricks (cleaning, aggregation, enrichment).

Save transformed data into ADLS Gen2 (processed zone).

Load into Synapse for querying.

Create dashboards in Power BI/Tableau/Fabric for decision-making.

📊 Use Cases

E-commerce sales trend analysis

Customer behavior insights

Product performance tracking

Business reporting & visualization
