---
title: 'TechLab: Develop Scalable Data Solutions with SQL Database in Microsoft Fabric'
layout: default
nav_order: 64
parent: 'Lab summaries'
---

**ID** 192172  
**Number:** LAB363  
**Name:** TechLab: Develop Scalable Data Solutions with SQL Database in Microsoft Fabric  
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** DREAM Labs Build, TrialFabricUsers, E5  

---

## Exercise Summary

**Exercise 1: Loading Data into SQL Database in Fabric**
- **Goal:** Set up a Microsoft Fabric workspace and SQL Database, then load and validate data from Azure SQL Database.
- **Actions:**
  - Sign in to Azure and verify resource group deployment.
  - Create a new Microsoft Fabric workspace and SQL Database.
  - Use a Fabric pipeline to ingest data from Azure SQL DB to Fabric SQL Database.
  - Validate schema compatibility and data transfer.
  - Query tables to confirm data presence.
- **Validation:**
  - Deployment status shows "1 Succeeded" in Azure portal.
  - Data is visible and queryable in the Fabric SQL Database.

**Exercise 2: Introduction to Copilot for SQL Database in Fabric**
- **Goal:** Leverage Copilot to assist with writing, correcting, and generating SQL queries in Microsoft Fabric.
- **Actions:**
  - Use Copilot suggestions to complete SQL queries in the editor.
  - Fix query errors using Copilot's Quick Actions.
  - Generate SQL queries from natural language prompts via Copilot chat.
- **Validation:**
  - Copilot suggestions are accepted and executed successfully.
  - Errors are resolved and correct results are returned for queries.

**Exercise 3: Exploring GraphQL API Endpoints in Microsoft Fabric**
- **Goal:** Create and expose a GraphQL API endpoint from a SQL Database in Microsoft Fabric and consume it in an application.
- **Actions:**
  - Create a SQL view for use in the GraphQL API.
  - Generate a GraphQL API from the view and expose it.
  - Select and load data objects into the GraphQL schema.
  - Write and test GraphQL queries in the Fabric portal.
  - Copy the GraphQL endpoint and integrate it into an ASP.NET web application.
- **Validation:**
  - GraphQL queries return expected JSON results in the portal.
  - Web application successfully queries the endpoint and displays results.

**Exercise 4: Data Serving in Fabric (Optional)**
- **Goal:** Build Power BI reports and semantic models from Fabric SQL Database data, using Copilot for insights and automation.
- **Actions:**
  - Create a semantic model from SQL Database data in Power BI.
  - Enable Q&A and Copilot features in Power BI settings.
  - Use Copilot to analyze data, generate reports, and create executive summaries.
- **Validation:**
  - Semantic model and reports are created and visible in Power BI.
  - Copilot provides insights and summaries as expected.

**Exercise 5: RAG Implementation with Azure OpenAI in Database (Optional)**
- **Goal:** Implement Retrieval-Augmented Generation (RAG) using Microsoft Fabric SQL Database as a vector store and Azure OpenAI for embeddings and natural language responses.
- **Actions:**
  - Retrieve Azure OpenAI endpoint and key from Azure portal.
  - Configure Fabric SQL Database for secure REST API calls to Azure OpenAI.
  - Create procedures for generating embeddings and storing them in the database.
  - Build procedures for similarity search and natural language response generation using GPT-4.
  - Test the RAG workflow by querying for relevant products and generating AI-powered responses.
- **Validation:**
  - Embeddings and chat messages are stored and retrievable in the database.
  - AI responses are generated and returned for user queries.
