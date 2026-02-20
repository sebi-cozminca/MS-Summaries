---
title: 'Scaling AI Experiences with Microsoft Foundry & Fabric Data Agent'
layout: default
nav_order: 48
parent: 'Lab summaries'
---

**ID** 208630  
**Number:** LAB 256  
**Name:** Scaling AI Experiences with Microsoft Foundry & Fabric Data Agent  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** M365Copilot, CopilotStudio, E3, Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Environment and Workspace Setup**
- **Goal:** Establish a Microsoft Fabric workspace and prepare the lab environment.
- **Actions:**
  - Log into the provided virtual machine and access the Microsoft Fabric portal.
  - Create a new Fabric workspace and Lakehouse.
  - Import and attach the setup notebook to the Lakehouse.
  - Execute the notebook to generate and verify Lakehouse data tables.
- **Validation:**
  - Confirm workspace and Lakehouse creation; verify presence of required tables with data in the Lakehouse.

**Exercise 2: Data Agent Creation and Configuration**
- **Goal:** Deploy and configure a Data Agent connected to the Lakehouse.
- **Actions:**
  - Create a Data Agent in the Fabric workspace.
  - Connect the Lakehouse as a data source and select all relevant tables.
  - Add agent instructions and data source instructions from provided text files.
  - Import example queries from a JSON file.
  - Publish the Data Agent and obtain the published URL.
- **Validation:**
  - Data Agent interface shows connected Lakehouse and tables; agent instructions and example queries are present; published URL is accessible.

**Exercise 3: Data Agent Testing**
- **Goal:** Validate Data Agent functionality through sample queries.
- **Actions:**
  - Interact with the Data Agent chat interface using a provided analytics question.
- **Validation:**
  - Agent returns a relevant response to the test query.

**Exercise 4: Local Development Environment Setup**
- **Goal:** Prepare the local development environment for application integration.
- **Actions:**
  - Open the project folder in VS Code and install required extensions (Python, Jupyter, Azure App Service).
  - Create and activate a Python virtual environment.
  - Install dependencies from requirements.txt.
  - Configure environment variables in .env and .env.example files.
- **Validation:**
  - All dependencies installed; .env file populated with required values.

**Exercise 5: Azure Service Configuration**
- **Goal:** Gather and configure Azure service credentials for application integration.
- **Actions:**
  - Retrieve and record endpoints, keys, and connection strings for Azure OpenAI, AI Search, Document Intelligence, Storage Account, Application Insights, Microsoft Fabric, and Tenant ID from the Azure portal.
  - Populate these values in the .env file.
- **Validation:**
  - .env file contains all required Azure service configuration values.

**Exercise 6: Data Indexing and Application Execution**
- **Goal:** Index source data and run the application for end-to-end validation.
- **Actions:**
  - Run scripts to create a search index and ingest documents.
  - Execute the provided Jupyter notebook for workflow validation.
  - Run the Streamlit application locally and test with sample queries.
- **Validation:**
  - Index and data ingestion complete; notebook runs successfully; Streamlit app responds to sample queries as expected.

**Exercise 7: (Optional) Azure Deployment**
- **Goal:** Deploy the application to Azure App Service.
- **Actions:**
  - Create deployment scripts and configuration files.
  - Deploy the application using VS Code Azure integration.
  - Set environment variables in the Azure portal.
  - Access the deployed app and review logs in Application Insights.
- **Validation:**
  - Application is accessible via Azure App Service; logs are available in Application Insights.
