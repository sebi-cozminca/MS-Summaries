---
title: 'TechLab: Modernize your data estate MS Fabric, Azure Databricks and AI Foundry'
layout: default
nav_order: 75
parent: 'Lab summaries'
---

**ID** 186880  
**Number:** LAB364  
**Name:** TechLab: Modernize your data estate MS Fabric, Azure Databricks and AI Foundry  
**CloudSubscriptionPoolName:** MS Learn CSS Production MCA  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Data Engineering and Data Factory Experience – Ingest Data from Analytical Data Sources into OneLake**
- **Goal:** Ingest and prepare data from multiple sources into Microsoft Fabric's OneLake for unified analytics.
- **Actions:**
  - Create a Microsoft Fabric-enabled workspace and add a lakehouse.
  - Create shortcuts to reference external data in ADLS Gen2 without copying.
  - Use Spark notebooks to create Delta tables from ingested data.
- **Validation:** Lakehouse and Delta tables are created and populated; data is accessible and visible in Fabric.

**Exercise 2: Azure Databricks Integration with Fabric – DLT Pipelines, Unity Catalog, and Mirrored Catalog**
- **Goal:** Integrate Azure Databricks with Microsoft Fabric for data transformation, governance, and seamless analytics.
- **Actions:**
  - Create a Delta Live Table (DLT) pipeline for data transformation in Databricks.
  - Explore and govern data using Unity Catalog in Databricks (via click-through exercise).
  - Mirror the Azure Databricks Catalog in Fabric and analyze data using T-SQL.
- **Validation:** DLT pipeline completes successfully; mirrored catalog tables are accessible and queries return expected results in Fabric.

**Exercise 3: Building an AI-Powered Chatbot with Microsoft Fabric and Azure AI Foundry**
- **Goal:** Integrate Fabric data with Azure AI Foundry and build an AI-powered chatbot for business insights.
- **Actions:**
  - Integrate Fabric data with Azure AI Foundry using Azure AI Search.
  - Establish Azure OpenAI and AI Search connections in Azure AI Foundry.
  - Set up and use Prompt Flow in Azure AI Foundry; deploy and test a shopping assistant chatbot.
- **Validation:** AI Search index is created and populated; connections to OpenAI and AI Search are established; chatbot responds accurately to queries.

**Exercise 4: Explore Data Science Experience in Microsoft Fabric**
- **Goal:** Enable end-to-end data science workflows and generative AI experiences in Microsoft Fabric.
- **Actions:**
  - Build and run ML models and experiments using Copilot in Fabric notebooks.
  - Implement a Data Agent for conversational Q&A over business data, including custom prompts and example queries.
- **Validation:** ML models run and return results; Data Agent answers business questions accurately and can be published for broader use.
