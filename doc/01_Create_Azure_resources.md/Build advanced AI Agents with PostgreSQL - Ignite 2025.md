---
title: 'Build advanced AI Agents with PostgreSQL - Ignite 2025'
layout: default
nav_order: 7
parent: 'Lab summaries'
---

**ID** 205227  
**Number:** LAB515  
**Name:** Build advanced AI Agents with PostgreSQL - Ignite 2025  
**CloudSubscriptionPoolName:** LAB426 Recycling CSS Pool  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** TrialFabricUsers  

---

## Exercise Summary

**Part 0: Log into Azure and Explore Azure Resources**
- **Goal:** Access the lab environment and review Azure resources for the agentic app.
- **Actions:**
  - Log into the VM and Azure Portal using provided credentials and Temporary Access Pass (TAP).
  - Identify the Azure OpenAI and Azure PostgreSQL Database resources in the portal.
- **Validation:**
  - Successful login and confirmation that both required resources are visible in the Azure Portal.

**Part 1: Setup your Azure PostgreSQL Database for your Agentic App**
- **Goal:** Connect to and configure the Azure PostgreSQL database for AI integration.
- **Actions:**
  - Open VS Code and use the PostgreSQL extension to connect to the Azure PostgreSQL database with Entra ID authentication.
  - Launch the PSQL command line shell and run scripts to create and populate tables with sample data.
  - Install and configure the azure_ai extension, set up connection to Azure OpenAI, and verify extension settings.
  - Review and use the azure_openai schema to generate vector embeddings for text data.
- **Validation:**
  - Database connection is established, sample data is loaded, extensions are installed, and embeddings can be generated and previewed.

**Part 2: Using AI-driven features in Postgres**
- **Goal:** Leverage AI and vector search capabilities within PostgreSQL for advanced data analysis.
- **Actions:**
  - Use SQL pattern matching (ILIKE) for basic text search.
  - Install the vector and pg_diskann extensions, add vector columns, and generate embeddings for case data.
  - Create a DiskANN index for efficient vector search.
  - Perform semantic search queries using vector similarity and Azure OpenAI embeddings.
- **Validation:**
  - Semantic search returns relevant results even when exact keywords are not present; vector operations and indexing are functional.

**Part 3: Build the Agentic App**
- **Goal:** Develop an agentic application that utilizes PostgreSQL AI features.
- **Actions:**
  - Open the provided Jupyter notebook (lab.ipynb) in VS Code.
  - Follow notebook instructions to implement and test the agentic app using the configured database and AI features.
- **Validation:**
  - Notebook runs successfully, and the agentic app demonstrates AI-driven data processing and analysis as described in the lab.
