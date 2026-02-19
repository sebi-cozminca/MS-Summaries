---
title: 'TechLab: Integrating Databricks and Fabric for Enhanced Analytical Solutions'
layout: default
nav_order: 72
parent: 'Lab summaries'
---

**ID** 169917
**Number:** 41-411-6
**Name:** TechLab: Integrating Databricks and Fabric for Enhanced Analytical Solutions
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** E5

---

# TechLab Integrating Databricks and Fabric for Enhanced Analytical Solutions – Lab Instruction Summary

## Exercise Summary

**Exercise 1: Getting Started – Environment Setup**
- **Goal:** Prepare the environment for secure integration between Azure Databricks and Microsoft Fabric.
- **Actions:**
  - Configure a service principal and secret in Entra ID.
  - Create an Azure Key Vault and store the client secret.
  - Enable SQL Server access for Fabric pipelines.
  - Add a Lakehouse container and medallion directories to ADLS Gen2 storage.
- **Validation:** Service principal, Key Vault, SQL access, and storage structure are configured and accessible.

**Exercise 2: Create a Fabric Workspace and Data Pipeline**
- **Goal:** Establish a Fabric workspace and ingest data into Lakehouses using data pipelines.
- **Actions:**
  - Create a Fabric-enabled workspace and three Lakehouses (bronze, silver, gold).
  - Use data pipelines to ingest data from Azure SQL DB to the bronze layer in ADLS Gen2.
- **Validation:** Data is ingested and visible in the bronze Lakehouse directory.

**Exercise 3: Establish Connectivity Between Databricks and ADLS Gen2**
- **Goal:** Enable secure access from Databricks to ADLS Gen2 using Key Vault-backed secrets.
- **Actions:**
  - Create a Databricks secret scope backed by Azure Key Vault.
  - Configure and test Databricks cluster connectivity to ADLS Gen2 using service principal credentials.
- **Validation:** Databricks can list and access data in the medallion container in ADLS Gen2.

**Exercise 4: Implement the Medallion Architecture Using Databricks**
- **Goal:** Transform and model data through bronze, silver, and gold layers using Databricks notebooks.
- **Actions:**
  - Import and run notebooks to read from bronze, convert to delta format, and write to silver.
  - Build data models and write curated data to the gold layer as external tables.
- **Validation:** Delta files are present in silver and gold directories; data models are created and verified.

**Exercise 5: Serving Data with Microsoft Fabric**
- **Goal:** Integrate gold layer data into Fabric Lakehouse and optimize for analytics.
- **Actions:**
  - Create a Lakehouse shortcut to the gold layer in ADLS Gen2.
  - Run maintenance commands (OPTIMIZE, V-order) on gold tables for performance.
- **Validation:** Shortcuts are created and tables are optimized for fast querying in Fabric.

**Exercise 6: Creating and Configuring the Semantic Model**
- **Goal:** Build a semantic model in Fabric for business analytics.
- **Actions:**
  - Create a new semantic model and select required tables from the Lakehouse.
  - Establish relationships between fact and dimension tables.
- **Validation:** Semantic model is created, relationships are established, and tables are ready for reporting.

**Exercise 7: Visualize the Data with Power BI**
- **Goal:** Create Power BI reports using the semantic model and direct lake mode.
- **Actions:**
  - Build a Power BI report with visualizations (e.g., top 10 customers by sales).
  - Apply filters and formatting to enhance report insights.
- **Validation:** Power BI report displays real-time analytics from the semantic model; visualizations are functional.

**Exercise 8: Lab Completion**
- **Goal:** Complete the lab and submit for credit.
- **Actions:**
  - Answer survey questions and select End to mark the lab as complete.
- **Validation:** Lab completion is recorded and feedback is submitted.
