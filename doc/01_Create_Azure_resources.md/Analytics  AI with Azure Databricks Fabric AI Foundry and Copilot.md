---
title: 'Analytics & AI with Azure Databricks, Fabric, AI Foundry and Copilot'
layout: default
nav_order: 1
parent: 'Lab summaries'
---

**ID** 205505  
**Number:** LAB 257  
**Name:** Analytics & AI with Azure Databricks, Fabric, AI Foundry and Copilot  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-MSLEARN-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** E5, TeamsEnt, CopilotStudioTrial, Ignite25Lab535Databricks 

---

## Exercise Summary

**Exercise 1: Lakehouse Setup & Data Orchestration with Azure Databricks and Lakeflow Spark Declarative Pipelines**
- **Goal:** Establish a unified analytics environment using Azure Databricks and orchestrate data pipelines for data transformation.
- **Actions:**
  - Log into Azure portal and Databricks workspace.
  - Create a schema and volume in Unity Catalog; upload raw data files.
  - Import and update a Databricks notebook for ETL pipeline configuration.
  - Create and run a Lakeflow Spark declarative pipeline for data transformation.
  - Use AI to generate column-level insights and review data lineage and profiling.
- **Validation:**
  - Successful upload of data, execution of ETL pipeline, and AI-generated column descriptions visible in Databricks.

**Exercise 2: AI-Driven Insights with Microsoft Foundry & Genie**
- **Goal:** Enable AI-powered analytics by integrating Databricks Genie with Microsoft Foundry and deploying an agent for business Q&A.
- **Actions:**
  - Create a Genie workspace in Databricks and configure it with the gold_transactions table.
  - Interact with Genie to generate insights and retrieve the Space ID.
  - Enable Managed MCP Servers in the workspace and connect Genie as a tool in Microsoft Foundry.
  - Create and configure an agent in Foundry, linking it to Genie for transaction analysis.
  - Test the agent in the Foundry Playground by querying for insights.
- **Validation:**
  - Agent responds to business questions using Genie and provides accurate, AI-driven insights in the Playground.

**Exercise 3: Azure Databricks Mirrored Catalog in Microsoft Fabric**
- **Goal:** Mirror Databricks Unity Catalog tables into Microsoft Fabric's OneLake and build semantic models for Power BI analytics.
- **Actions:**
  - Create a new workspace in Microsoft Fabric and set up a mirrored Azure Databricks catalog connection using service principal credentials.
  - Select and sync the required schema and tables.
  - Create a semantic model in Direct Lake mode using the mirrored data.
  - Use Power BI Copilot to generate and analyze reports on fraudulent transactions.
- **Validation:**
  - Mirrored tables are accessible in Fabric; semantic model and Power BI reports are generated and display actionable insights.

**Exercise 4: Copilot Studio for Low-Code Automation (Optional)**
- **Goal:** Build and publish a Copilot Studio agent that leverages Databricks data for business Q&A and integrates with Microsoft Teams.
- **Actions:**
  - Create and configure a new agent in Copilot Studio, connecting it to Azure Databricks as a knowledge source.
  - Test the agent with business questions to validate data connectivity and response quality.
  - Publish the agent and add it to Microsoft Teams as a channel.
  - Upload the Teams app package and interact with the agent in Teams.
- **Validation:**
  - Agent responds accurately to business queries in Copilot Studio and Teams, using Databricks data with citations.
