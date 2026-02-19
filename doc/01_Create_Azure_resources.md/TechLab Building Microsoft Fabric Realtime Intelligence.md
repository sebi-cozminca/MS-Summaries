---
title: 'TechLab: Building Microsoft Fabric Realtime Intelligence'
layout: default
nav_order: 58
parent: 'Lab summaries'
---

**ID** 188046
**Number:** 41-411-7
**Name:** TechLab: Building Microsoft Fabric Realtime Intelligence
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** E5

---

# Tech Mastery Catalog Lab Instruction Summary

## Exercise Summary

**Exercise 1: Configure Pre-requisites**
- **Goal:** Prepare the Microsoft Fabric environment and review foundational concepts for Real-Time Intelligence.
- **Actions:**
  - Review KQL and Real-Time Intelligence documentation.
  - Sign in to the lab VM and Microsoft Fabric portal.
  - Create a Fabric workspace with Fabric capacity.
- **Validation:** Workspace is created and accessible in the Fabric portal.

**Exercise 2: Build Real-Time Data Architecture**
- **Goal:** Set up the medallion architecture using Eventhouse, Eventstream, and Lakehouse in Microsoft Fabric.
- **Actions:**
  - Create an Eventhouse for real-time data storage.
  - Set up an Eventstream with a custom endpoint for ingesting events.
  - Import and configure a data generator notebook to simulate streaming events.
  - Connect Eventstream to Eventhouse and configure the destination table.
  - Enable OneLake availability for KQL database tables.
  - Build the KQL database schema using provided scripts and shortcuts.
  - Create a Lakehouse and add shortcuts to KQL database tables.
- **Validation:** Streaming events are ingested and visible in Eventhouse; tables are accessible in both KQL database and Lakehouse.

**Exercise 3: Create and Run Data Pipelines**
- **Goal:** Ingest operational data from SQL DB into Eventhouse using Fabric Data Factory pipelines.
- **Actions:**
  - Configure and run pipelines to copy Address, Customer, SalesOrderHeader, and SalesOrderDetail tables from SQL DB to Eventhouse.
  - Map schemas and verify data import for each table.
  - Use update policies and materialized views for Silver and Gold layers.
- **Validation:** Data is successfully copied and transformed; Silver and Gold tables show expected row counts and columns.

**Exercise 4: Create a Real-Time Dashboard**
- **Goal:** Visualize streaming and batch data in real time using Fabric Real-Time Dashboards.
- **Actions:**
  - Create a Real-Time Dashboard and connect it to the Eventhouse/KQL database.
  - Add and configure visual tiles for Clicks by Hour, Impressions by Hour, and Average Page Load Time using KQL queries.
- **Validation:** Dashboard tiles display live, updating data; visualizations reflect real-time event ingestion and processing.
