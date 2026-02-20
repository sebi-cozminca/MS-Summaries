---
title: 'Analytics with Microsoft Fabric: Data to AI-Powered Insights - Ignite 2025'
layout: default
nav_order: 2
parent: 'Lab summaries'
---

**ID** 205504  
**Number:** LAB534  
**Name:** Analytics with Microsoft Fabric: Data to AI-Powered Insights - Ignite 2025  
**CloudSubscriptionPoolName:** Ignite 2025 - CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** M365Copilot, CopilotStudio, E3, E3 + PBI Pro  

---

## Exercise Summary

**Fabric Environment Setup:**
- **Goal:** Prepare the Microsoft Fabric environment and foundational data assets for the lab.
- **Actions:**
  - Create a new Fabric workspace and configure licensing.
  - Authenticate to Microsoft Fabric using Azure CLI in the VM terminal.
  - Run a C# script to automatically create a Fabric Data Warehouse and Lakehouse, and load initial data.
  - Verify creation of `fc_commerce_wh` (warehouse) and `fc_commerce_lh` (lakehouse) and preview loaded tables.
- **Validation:**
  - Workspace, warehouse, and lakehouse are visible in Fabric; tables are populated and data is previewable.

**Exercise 1: Provisioning Cosmos DB in Fabric (Operational Data Store)**
- **Goal:** Set up Cosmos DB in Fabric as the operational data store and load initial data.
- **Actions:**
  - Create a new Cosmos DB database (`fc_commerce_cosmos`) in the Fabric workspace.
  - Add a `customers` container with appropriate partition key.
  - Upload initial customer data from a JSON file.
  - Run SQL queries to validate data, analyze recommendations, and calculate membership tiers.
- **Validation:**
  - Data is loaded and queries return expected results in the Cosmos DB container.

**Exercise 2: Batch Data Loading and Cross-Database Analytics (Cosmos DB to Data Warehouse)**
- **Goal:** Enable analytics by leveraging Cosmos DB's automatic mirroring to OneLake and perform cross-database queries.
- **Actions:**
  - Monitor Cosmos DB replication to OneLake and access mirrored data via SQL endpoint.
  - Run T-SQL queries to analyze customer preferences.
  - Join Cosmos DB and Data Warehouse data for cross-database analytics (e.g., favorite drinks, revenue, loyalty).
  - Create Lakehouse shortcuts to Cosmos DB tables and analyze with Spark SQL in notebooks.
- **Validation:**
  - Successful execution of cross-database queries and analytics in both SQL endpoint and Lakehouse notebook.

**Exercise 3: Real-Time Streaming of POS Events**
- **Goal:** Ingest and analyze real-time POS event data using Eventstream, Eventhouse, and KQL in Fabric.
- **Actions:**
  - Run a C# script to generate and stream POS data.
  - Create an Eventhouse (`fc_commerce_eventhouse`) and connect Eventstream output to it.
  - Configure KQL destination table (`transactions_live`) and activate ingestion.
  - Query Eventhouse to verify live data ingestion.
  - Build Silver layer KQL functions for analytics and run queries for sales insights.
- **Validation:**
  - Real-time data appears in Eventhouse; KQL queries and Silver layer analytics return expected results.

**Exercise 4: Implement Reverse ETL and Build Personalization Model**
- **Goal:** Transform streaming data, update Cosmos DB with enriched insights, and build a personalization model using Fabric Notebooks.
- **Actions:**
  - Create SQL views in the Data Warehouse for dimensional modeling.
  - Import and run Fabric Notebooks to transform data and stage it in Lakehouse (Parquet files).
  - Load transformed data into warehouse tables using SQL COPY INTO from Parquet.
  - Run a second notebook to perform Reverse ETL, updating Cosmos DB with enriched profiles and building a recommendation model.
  - Validate updates by querying Cosmos DB for new profile data.
- **Validation:**
  - Data warehouse tables and Cosmos DB profiles reflect transformed and enriched data; recommendation model is built.

**Exercise 5 (Optional): Serve Personalized Recommendations from Cosmos DB**
- **Goal:** Deploy and run a demo application that serves AI-powered recommendations from Cosmos DB.
- **Actions:**
  - Configure the app with the Cosmos DB endpoint.
  - Run the .NET Blazor application to serve recommendations to users.
- **Validation:**
  - Application runs and displays personalized menu item recommendations based on Cosmos DB data.
