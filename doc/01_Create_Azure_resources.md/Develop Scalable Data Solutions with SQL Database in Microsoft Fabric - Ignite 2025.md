---
title: 'Develop Scalable Data Solutions with SQL Database in Microsoft Fabric - Ignite 2025'
layout: default
nav_order: 22
parent: 'Lab summaries'
---

**ID** 205171
**Number:** LAB533
**Name:** Develop Scalable Data Solutions with SQL Database in Microsoft Fabric - Ignite 2025
**CloudSubscriptionPoolName:** Ignite 2025 - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** M365Copilot, CopilotStudio, E5

---

# Exercise Summary

**Exercise 1: Introduction to SQL Database in Microsoft Fabric**
- **Goal:** Set up and explore a SQL database within Microsoft Fabric.
- **Actions:**
  - Log in to the Microsoft Fabric portal and create a new workspace.
  - Create a SQL database in the workspace and load it with sample data.
  - Explore the database using the Database Explorer and Query Editor.
  - Access and use the SQL analytics endpoint for cross-database queries and monitor replication status.
- **Validation:**
  - Database and workspace are created; sample data is loaded and accessible; queries return expected results.

**Exercise 2: Copilot Capabilities for SQL Database in Microsoft Fabric**
- **Goal:** Leverage Copilot to enhance SQL query development and troubleshooting.
- **Actions:**
  - Use Copilot in the query editor for auto-suggestions, error fixing, and query explanations.
  - Interact with Copilot's chat pane for natural language to SQL conversion and direct query execution.
  - Approve and execute Copilot-generated queries and create database views.
- **Validation:**
  - Copilot suggestions and fixes are applied; queries execute successfully; Copilot-generated views and results are validated in the database.

**Exercise 3: RAG Implementation with Azure OpenAI**
- **Goal:** Implement Retrieval-Augmented Generation (RAG) using SQL database and Azure OpenAI.
- **Actions:**
  - Set up database credentials for Azure OpenAI integration.
  - Add vector columns to tables and create stored procedures for generating embeddings.
  - Generate and store embeddings for product data; perform vector similarity searches using VECTOR_DISTANCE.
  - Create and test stored procedures for semantic search and product recommendations.
- **Validation:**
  - Embeddings are created and stored; similarity search returns relevant results; stored procedures execute and return expected outputs.

**Exercise 4: Build a GraphQL API for RAG Applications**
- **Goal:** Expose RAG capabilities via a GraphQL API integrated with Azure OpenAI.
- **Actions:**
  - Create stored procedures for chat completion using Azure OpenAI and product data.
  - Wrap procedures for GraphQL API consumption and deploy the API in Microsoft Fabric.
  - Test the API using the GraphQL query editor and validate AI-generated responses.
- **Validation:**
  - GraphQL API returns relevant, AI-generated answers to product queries; integration with stored procedures and OpenAI is successful.

**Exercise 5: Power BI Report Using Semantic Model**
- **Goal:** Build Power BI reports from SQL analytics endpoint data using Copilot.
- **Actions:**
  - Create a semantic model from the SQL analytics endpoint in Fabric.
  - Use Copilot to suggest and generate report content in Power BI.
  - Create and customize reports based on Copilot's suggestions.
- **Validation:**
  - Power BI reports are generated and display data from the semantic model; Copilot suggestions are reflected in the report content.

**Lab Completion**
- **Goal:** Review and reinforce key concepts and provide feedback.
- **Actions:**
  - Complete the lab feedback survey and explore additional documentation and community resources.
- **Validation:**
  - Feedback is submitted; participants have access to further learning materials and community links.
