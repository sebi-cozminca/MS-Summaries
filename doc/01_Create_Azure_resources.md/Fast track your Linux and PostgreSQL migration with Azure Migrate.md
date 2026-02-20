---
title: 'Fast track your Linux and PostgreSQL migration with Azure Migrate'
layout: default
nav_order: 25
parent: 'Lab summaries'
---

**ID** 208614  
**Number:** LAB 109  
**Name:** Fast track your Linux and PostgreSQL migration with Azure Migrate  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** M365Copilot, CopilotStudio, Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Prepare for Workload Migration with Azure Migrate**
- **Goal:** Establish Azure Migrate projects and configure discovery and migration for Linux workloads.
- **Actions:**
  - Create two Azure Migrate projects for discovery/assessment and VM migration.
  - Import offline discovery data and configure Hyper-V host registration.
  - Set up agent-based replication for application-tier VM migration.
- **Validation:**
  - Both Azure Migrate projects are accessible; inventory is populated; Hyper-V host is registered and healthy.

**Exercise 2: Define the Application and Create a Business Case**
- **Goal:** Plan migration by grouping workloads, generating a business case, and building a migration wave plan.
- **Actions:**
  - Define an application for the Airsonic stack, linking frontend/backend servers and workloads.
  - Build a business case to estimate costs, savings, and migration strategies.
  - Review discovered inventory and assessment outputs for modernization options.
  - Create a wave plan from the recommended path and add migration tasks.
  - (Optional) Document identity mapping from FreeIPA to Microsoft Entra ID.
- **Validation:**
  - Application, business case, assessment, and wave plan are created and reflect expected scope; identity mapping is documented.

**Exercise 3: Migrate PostgreSQL to Azure Database for PostgreSQL Flexible Server**
- **Goal:** Migrate the backend database to Azure PaaS with secure connectivity and validation.
- **Actions:**
  - Establish VPN connectivity for private access to Azure resources.
  - Update and mark application data for migration validation.
  - Retrieve internal IP of the Flexible PostgreSQL server via Private DNS.
  - Run validation and offline migration jobs for the database.
  - Update application configuration to use the new database endpoint and reboot the server.
- **Validation:**
  - Database migration job completes successfully; application connects to the new database and retains pre-migration data.

**Exercise 4: Migrate Linux Middleware Using Azure Migrate**
- **Goal:** Replicate and migrate the Airsonic frontend VM to Azure IaaS.
- **Actions:**
  - Start replication for the Airsonic-Frontend VM and monitor until protected.
  - Initiate planned migration (failover) and approve VM shutdown for cutover.
  - Stop replication after migration and validate application functionality on the Azure VM.
- **Validation:**
  - VM migration completes; application is accessible on the Azure VM and connected to the migrated database; replication state is cleaned up.
