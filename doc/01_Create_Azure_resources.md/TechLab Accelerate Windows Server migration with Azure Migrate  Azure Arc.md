---
title: 'TechLab: Accelerate Windows Server migration with Azure Migrate & Azure Arc'
layout: default
nav_order: 50
parent: 'Lab summaries'
---

**ID** 186373  
**Number:** TechConnect Lab315  
**Name:** TechLab: Accelerate Windows Server migration with Azure Migrate & Azure Arc  
**CloudSubscriptionPoolName:** TechMastery - CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Prepare to Onboard Server to Azure Arc and Create Log Analytics Workspace**
- **Goal:** Prepare a Windows Server for Azure Arc onboarding and provision a Log Analytics workspace.
- **Actions:**
  - Log in to the Windows VM and Azure portal with provided credentials.
  - Register required resource providers in the Azure subscription.
  - Deploy the Azure Arc resource group template.
  - Create a Log Analytics workspace in the specified resource group and region.
- **Validation:**
  - Resource providers show as registered; Log Analytics workspace is created and visible in the portal.

**Exercise 2: Onboard Server to Azure Arc**
- **Goal:** Connect the Windows Server to Azure Arc and deploy the AMA extension.
- **Actions:**
  - Use the Azure portal to generate and run the onboarding script on the server.
  - Complete interactive device login and confirm Arc agent connection.
- **Validation:**
  - Server appears in Azure Arc with agent status as 'Connected'.

**Exercise 3: Azure Migrate Assessment and Business Case with Azure Arc**
- **Goal:** Generate a business case for Azure Arc-enabled workloads using Azure Migrate.
- **Actions:**
  - Create an Azure Migrate project and import the provided CSV data.
  - Build a business case with specified settings (location, savings options, discount).
  - Review cost projections and insights for Arc-enabled migration.
- **Validation:**
  - Business case status shows 'Completed'; cost projections and insights are viewable in the portal.

**Exercise 4: Activate Windows Server Management Enabled by Azure Arc**
- **Goal:** Enable Windows Server management features for Arc-enabled servers.
- **Actions:**
  - Navigate to Azure Arc licenses and activate Azure benefits for the target server.
- **Validation:**
  - Azure benefits are shown as activated on the server's overview page.

**Exercise 5: Deploy Azure Management Services Using At-Scale Solution Onboarding**
- **Goal:** Enable management services (Update Manager, Change Tracking) for Arc-enabled servers at scale.
- **Actions:**
  - Use the at-scale onboarding portal to enable Azure Update Manager and Change Tracking & Inventory.
  - Assign the Log Analytics workspace and confirm service enablement.
- **Validation:**
  - Services are enabled and visible under the server's Operations section in Azure Arc.

**Exercise 6: Apply Azure Policy with Machine Configuration**
- **Goal:** Enforce security baselines on Arc-enabled servers using Azure Policy.
- **Actions:**
  - Assign the 'Windows machines should meet requirements of the Azure compute security baseline' policy to the server.
  - Include Arc Connected Servers in the policy scope.
- **Validation:**
  - Policy assignment is created and visible in the server's Policies section.

**Exercise 7: Azure Update Manager**
- **Goal:** Assess and manage updates for Arc-enabled servers using Azure Update Manager.
- **Actions:**
  - Use Azure Update Manager to check for updates on the connected server.
- **Validation:**
  - Update assessment results are displayed for the server in the portal.

**Exercise 8: Get Involved with Azure Arc Community**
- **Goal:** Join the Azure Arc community for ongoing learning and updates.
- **Actions:**
  - Visit the provided link to sign up for the Azure Arc community call and newsletter.
- **Validation:**
  - Successful signup for the community call/newsletter.
