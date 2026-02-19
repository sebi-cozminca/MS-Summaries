---
title: 'TechLab: Using Copilots with Various Fabric Workloads'
layout: default
nav_order: 86
parent: 'Lab summaries'
---

**ID** 168496
**Number:** 41-411-6
**Name:** TechLab: Using Copilots with Various Fabric Workloads
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS
**AllowSave:** True
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** E5

---

# Exercise Summary

**Lab Setup: Create a Workspace**
- **Goal:** Set up the Microsoft Fabric environment for data analytics and Copilot usage.
- **Actions:**
  - Sign in to the lab VM and Power BI portal.
  - Create a new Fabric workspace named for the lab instance.
  - Verify Fabric workspace type and capacity.
- **Validation:**
  - Workspace is created and accessible in Power BI/Fabric.

**Exercise 1: Ingest a Dataset into Fabric by using Data Pipelines Copilot**
- **Goal:** Ingest and explore data using Copilot in Fabric Data Pipelines.
- **Actions:**
  - Create a Lakehouse and Dataflow Gen2 for the Northwind dataset.
  - Connect to an OData source and select relevant tables.
  - Use Copilot to filter, aggregate, and transform data with natural language prompts.
  - Publish the ingested data.
- **Validation:**
  - Data is loaded, transformed, and published to the Lakehouse; results are visible in the workspace.

**Exercise 2: Move and Transform Dataset to a Data Warehouse with Dataflow Gen 2 Copilot**
- **Goal:** Move and transform data into a Fabric Data Warehouse using Copilot and SQL queries.
- **Actions:**
  - Create a new Data Warehouse and load sample data.
  - Use Copilot to generate and run SQL queries, including troubleshooting and code explanation features.
  - Build queries from comments and natural language, and refine results as needed.
- **Validation:**
  - Queries execute successfully and return expected results; Copilot assists with query generation and error correction.

**Exercise 3: Move Dataset(s) to Lakehouse via Notebook and Copilot**
- **Goal:** Use Copilot in Fabric Notebooks to load, analyze, and visualize data.
- **Actions:**
  - Open a Lakehouse and create a new notebook.
  - Use Copilot to generate code for loading data into DataFrames and displaying results.
  - Leverage Copilot for code completion, debugging, and documentation.
  - Install required packages and resolve code errors as guided by Copilot.
- **Validation:**
  - Data is loaded and visualized (e.g., word cloud); notebook cells execute without errors.

**Exercise 4: Reporting with Power BI Copilot**
- **Goal:** Create and enhance Power BI reports using Copilot for data from the Data Warehouse and Lakehouse.
- **Actions:**
  - Create new reports and pages using Copilot prompts.
  - Add visualizations and narrative insights, referencing visuals across report pages.
  - Save the report as "Executive Overview."
- **Validation:**
  - Reports and narratives are generated as specified; insights reference correct visuals and data.

**Surveys**
- **Goal:** Collect user feedback before and after the lab.
- **Actions:**
  - Complete pre-lab and post-lab surveys.
- **Validation:**
  - Surveys submitted; lab completion is recorded.