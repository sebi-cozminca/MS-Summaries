---
title: 'TechLab: App Service Migration Deep Dive'
layout: default
nav_order: 52
parent: 'Lab summaries'
---

**ID** 162929  
**Number:** 41-411-8  
**Name:** TechLab: App Service Migration Deep Dive  
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)  
**AllowSave:** True  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Assessment**
- **Goal:** Evaluate .NET applications for migration readiness to Azure App Service.
- **Actions:**
  - Use PowerShell scripts to assess IIS-hosted applications and generate readiness reports.
  - Analyze application source code with Azure Migrate application and code assessment tools.
  - Review generated reports for migration blockers and warnings.
- **Validation:**
  - ReadinessResults.json and HTML reports indicate migration status and issues for each application.

**Exercise 2: Prepare the Blazor Application for Migration**
- **Goal:** Package and configure the Blazor application for migration to Azure App Service.
- **Actions:**
  - Run scripts to package the Blazor site and generate migration settings.
  - Edit migration settings for unique site naming.
- **Validation:**
  - MigrationSettings.json is correctly configured and ready for use in migration.

**Exercise 3: Migrate the Blazor Application**
- **Goal:** Migrate the Blazor application to Azure App Service using automation.
- **Actions:**
  - Execute migration scripts to deploy the application to Azure.
  - Verify deployment in the Azure portal under the designated resource group.
- **Validation:**
  - App Service and App Service Plan are created; application is hosted in Azure and visible in the portal.

**Exercise 4: Migrate Enterprise Applications with .NET/Initiate Technical Assessment**
- **Goal:** Explore scaling, monitoring, and performance features for migrated .NET applications in Azure App Service.
- **Actions:**
  - Configure automatic scaling for the App Service.
  - Enable Application Insights for monitoring and set up availability tests.
  - Configure Azure Load Testing to simulate load and observe scaling behavior.
  - Query performance counters and review live metrics in Application Insights.
- **Validation:**
  - Scaling, monitoring, and load testing features are enabled; metrics and test results are visible in the Azure portal.

**Next Steps and Resources**
- **Goal:** Extend learning and apply migration best practices.
- **Actions:**
  - Review the migration checklist, reference architectures, and bulk assessment tools via provided links.
- **Validation:**
  - Access to additional resources and tools for future migration projects.
