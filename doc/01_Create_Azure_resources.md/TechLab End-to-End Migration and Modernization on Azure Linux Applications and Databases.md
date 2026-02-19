---
title: 'TechLab: End-to-End Migration and Modernization on Azure: Linux, Applications, and Databases'
layout: default
nav_order: 67
parent: 'Lab summaries'
---

**ID** 200711
**Number:** Lab313
**Name:** TechLab: End-to-End Migration and Modernization on Azure: Linux, Applications, and Databases
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Prepare for workload migration with Azure Migrate**
- **Goal:** Set up Azure Migrate and register an on-premises appliance to enable discovery and migration of Hyper-V workloads.
- **Actions:**
  - Prepare the Hyper-V host using a PowerShell script and configure network settings.
  - Provision Azure Migrate resources (resource group, storage account, virtual network) via Cloud Shell.
  - Create a new Azure Migrate project in the portal.
  - Register the Azure Migrate appliance with the project using the Appliance Configuration Manager.
- **Validation:**
  - Script runs without errors and network category is reset.
  - Azure resources are visible in the resource group.
  - Azure Migrate project and appliance registration are confirmed in the portal.

**Exercise 2: Provision Azure Database Migration Service**
- **Goal:** Deploy Azure Database Migration Service (DMS) and configure secure connectivity for SQL Server migration.
- **Actions:**
  - Create a new DMS instance in the correct resource group and region.
  - Download, install, and register a self-hosted integration runtime (SHIR) on the Lab VM.
  - Add the SHIR node's IP to the Azure SQL Database firewall.
- **Validation:**
  - DMS instance is deployed and accessible in the portal.
  - SHIR node appears as Online in Azure.
  - Firewall rule is created for SHIR IP.

**Exercise 3: Discover virtual machines and workloads on the Hyper-V host**
- **Goal:** Use Azure Migrate to discover VMs and workloads on the Hyper-V host, including guest-level details.
- **Actions:**
  - Add credentials and discovery sources in the Appliance Configuration Manager.
  - Enable guest discovery and provide multiple sets of credentials for workload inspection.
  - Start the discovery process and monitor progress.
- **Validation:**
  - Discovery completes and VMs/workloads appear in Azure Migrate inventory.

**Exercise 4: Prepare on-premises web apps for migration**
- **Goal:** Deploy an Azure App Service Plan and migrate a PHP web application to Azure App Service.
- **Actions:**
  - Use Azure Cloud Shell to clone the web app repository and deploy using `az webapp up` with PHP 8.2 on Linux.
  - Register the Microsoft.Web provider and authenticate as needed.
- **Validation:**
  - App Service Plan and web app are created and visible in the resource group.
  - Web app is accessible after deployment.

**Exercise 5: Perform Assessments of discovered resources**
- **Goal:** Assess migration readiness for Linux VMs and database workloads using Azure Migrate.
- **Actions:**
  - Review discovery results and create assessments for Linux VM, SQL Server, and PostgreSQL.
  - Configure assessment settings for target platforms and performance-based sizing.
  - Review assessment results for compatibility and sizing recommendations.
- **Validation:**
  - Assessments are created and visible in Azure Migrate.
  - Assessment results provide actionable recommendations.

**Exercise 6: Replicate the Linux Ubuntu VM to Azure**
- **Goal:** Enable and configure replication of a Hyper-V-based Ubuntu VM to Azure using Azure Migrate.
- **Actions:**
  - Review the assessment report for the Linux VM and confirm readiness.
  - Download and install the Azure Site Recovery provider and register the Hyper-V host.
  - Assign required roles to Recovery Services vault and storage account.
  - Start replication for the Linux VM from the Azure Migrate portal.
- **Validation:**
  - Replication provider is installed and host is registered.
  - Required role assignments are in place.
  - Replication process is initiated successfully in Azure Migrate.
