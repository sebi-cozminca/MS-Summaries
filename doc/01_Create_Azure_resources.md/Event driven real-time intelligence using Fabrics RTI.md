---
title: 'Event driven, real-time intelligence using Fabric's RTI'
layout: default
nav_order: 24
parent: 'Lab summaries'
---

**ID** 208628  
**Number:** LAB 255  
**Name:** Event driven, real-time intelligence using Fabric's RTI  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-MSLEARN-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** E5  

---

## Exercise Summary

**Exercise 1: Environment Setup**
- **Goal:** Establish the foundational infrastructure for real-time analytics using Microsoft Fabric and Eventhouse.
- **Actions:**
  - Sign in to Microsoft Fabric and create a new workspace.
  - Provision an Eventhouse and KQL database, enable OneLake availability.
- **Validation:**
  - Workspace and Eventhouse with KQL database are created and visible in the Fabric portal.

**Exercise 2: Verify CosmosDB Configuration**
- **Goal:** Confirm Azure Cosmos DB setup and retrieve connection details for analytics integration.
- **Actions:**
  - Access Azure Portal and verify CosmosDB resource, databases, and containers.
  - Retrieve and store URI, primary key, and connection string for later use.
- **Validation:**
  - CosmosDB resource is present with required databases and containers; connection details are available.

**Exercise 3: Create Event Generator Notebook**
- **Goal:** Populate Cosmos DB with simulated retail data for real-time analytics.
- **Actions:**
  - Import and configure the Event Generator notebook in Fabric.
  - Set CosmosDB connection parameters and run the notebook to generate events.
  - Verify event data appears in CosmosDB containers.
- **Validation:**
  - Events are visible in CosmosDB retail-events and customer-events containers.

**Exercise 4: Build Eventstream with CosmosDB Source**
- **Goal:** Create a real-time Eventstream pipeline from CosmosDB to Eventhouse for analytics.
- **Actions:**
  - Create an Eventstream and add CosmosDB sources for retail and customer events.
  - Configure transformations (filters, union, SQL code, manage fields) and destinations (Eventhouse tables).
  - Set up filters for event types and enrich data with additional fields.
  - Publish and verify the Eventstream pipeline.
- **Validation:**
  - Data flows from CosmosDB to Eventhouse tables; Eventstream and destinations are active and populated.

**Exercise 5: Real-Time Analytics and Transformations**
- **Goal:** Analyze and visualize real-time data using KQL queries, dashboards, and alerts.
- **Actions:**
  - Create KQL queries for revenue, customer metrics, and inventory alerts.
  - Build a real-time dashboard with visualizations for key metrics.
  - Configure Activator alerts for critical inventory drops.
- **Validation:**
  - Dashboard displays live analytics; alerts trigger on threshold conditions; KQL queries return expected results.

**Exercise 6: Write-back to Azure CosmosDB for In-App Analytics**
- **Goal:** Complete the analytics pipeline by writing enriched insights back to CosmosDB.
- **Actions:**
  - Import and run a Spark notebook to aggregate and transform data from Eventhouse.
  - Write results to CosmosDB containers for downstream consumption.
  - Verify enriched data in CosmosDB using Data Explorer.
- **Validation:**
  - Enriched insights are present in CosmosDB containers; notebook executes successfully and data is accessible.

**Optional: Further Exploration**
- **Goal:** Deepen understanding of real-time analytics with advanced exercises.
- **Actions:**
  - Modify time windows, create new aggregations, and perform data quality checks.
  - Analyze customer churn, product affinity, and implement real-time alerting logic.
  - Schedule and operationalize notebooks for production scenarios.
- **Validation:**
  - Custom queries and analytics run successfully; additional insights and operational features are validated.
