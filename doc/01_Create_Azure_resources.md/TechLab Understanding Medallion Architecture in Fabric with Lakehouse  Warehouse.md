---
title: 'TechLab: Understanding Medallion Architecture in Fabric with Lakehouse + Warehouse'
layout: default
nav_order: 82
parent: 'Lab summaries'
---

**ID** 168013  
**Number:** 41-411-6  
**Name:** TechLab: Understanding Medallion Architecture in Fabric with Lakehouse + Warehouse  
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** E5  

---

## Exercise Summary

**Exercise 1: Environment Setup**
- **Goal:** Set up access to Microsoft Fabric and create a workspace for medallion architecture.
- **Actions:**
  - Sign in to the lab VM and Microsoft Fabric portal.
  - Create a new Fabric workspace with specified settings.
- **Validation:**
  - Workspace is visible and accessible in the Fabric portal.

**Exercise 2: Set up the Medallion Architecture**
- **Goal:** Establish the bronze, silver, and gold layers using Lakehouses and a Data Warehouse.
- **Actions:**
  - Create two Lakehouses (bronze, silver) in the workspace.
  - Create a Data Warehouse (gold) in the workspace.
- **Validation:**
  - Both Lakehouses and the Data Warehouse are provisioned and listed in the workspace.

**Exercise 3: Ingest Data into the Bronze Layer**
- **Goal:** Ingest raw data into the bronze Lakehouse using Fabric Data Factory.
- **Actions:**
  - Create a data pipeline to copy data from Azure Blob Storage to the bronze Lakehouse.
  - Configure source and destination settings for the pipeline.
  - Run the pipeline and verify data ingestion.
- **Validation:**
  - Raw data appears in the bronze Lakehouse under the expected directory structure.

**Exercise 4: Transfer Data into the Silver Layer**
- **Goal:** Move and transform data from the bronze to the silver Lakehouse and create analytical tables.
- **Actions:**
  - Create a pipeline to transfer data from bronze to silver Lakehouse.
  - Use notebooks to create fact and dimension tables in the silver Lakehouse.
- **Validation:**
  - Fact and dimension tables are present in the silver Lakehouse and populated with data.

**Exercise 5: Configure and Populate the Data Warehouse**
- **Goal:** Set up schemas and tables in the Data Warehouse and orchestrate data loading from the silver Lakehouse.
- **Actions:**
  - Create schemas and tables using SQL scripts.
  - Use data pipelines and stored procedures to load and transform data into the warehouse.
  - Update pipelines to orchestrate table creation, data loading, and model refresh.
- **Validation:**
  - Data is loaded into stage and dbo schemas; record counts confirm successful transfer.

**Exercise 6: Analyze with Power BI**
- **Goal:** Build a semantic model and create a Power BI report for data analysis.
- **Actions:**
  - Create a semantic model including key tables and relationships.
  - Design a Power BI report with visualizations for profit analysis by territory and state.
- **Validation:**
  - Report displays correct data and updates visuals based on slicer selections.

**Lab Completion**
- **Validation:**
  - Submit the lab in the Skillable platform and confirm completion status in Viva and Learning Path the following week.
