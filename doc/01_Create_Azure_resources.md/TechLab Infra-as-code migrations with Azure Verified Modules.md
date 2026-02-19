---
title: 'TechLab: Infra-as-code migrations with Azure Verified Modules'
layout: default
nav_order: 71
parent: 'Lab summaries'
---

**ID** 186387
**Number:** TechConnect Lab310
**Name:** TechLab: Infra-as-code migrations with Azure Verified Modules
**CloudSubscriptionPoolName:** Ignite (CSS) - Prod
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# TechLab Infra-as-code Migrations with Azure Verified Modules – Lab Instruction Summary

## Exercise Summary

**Exercise 1: Azure Verified Modules from Scratch**
- **Goal:** Learn to find and leverage Azure Verified Modules (AVM) for deploying basic Azure architectures with Terraform.
- **Actions:**
  - Explore AVM website and module indexes.
  - Locate, review, and use module examples and submodules.
- **Validation:** Ability to identify and use AVM modules and examples for infrastructure deployment.

**Exercise 2: Set up Terraform Tooling and Lab Environment**
- **Goal:** Prepare the local environment for Terraform-based Azure deployments.
- **Actions:**
  - Update Terraform to the latest version and install required VS Code extensions.
  - Create lab folder structure and initialize a git repository.
  - Configure Azure CLI authentication and environment variables.
  - Set up .gitignore and commit initial files.
- **Validation:** Terraform, VS Code, and git are configured; initial repo structure is committed.

**Exercise 3: Deploy Azure Resources Using AVM Modules**
- **Goal:** Deploy a network, subnets, storage account, and private endpoint using AVM modules in Terraform.
- **Actions:**
  - Find and use AVM modules for Resource Group, Virtual Network, Subnets, and Storage Account.
  - Reference module outputs and variables across resources.
  - Use random_string for unique storage account names.
  - Format, plan, and apply Terraform configurations; commit after each resource deployment.
- **Validation:** Resources are deployed in Azure; each step is validated by successful Terraform apply and Azure Portal checks.

**Exercise 4: Validate and Check Deployed Infrastructure**
- **Goal:** Confirm successful deployment and configuration of all resources.
- **Actions:**
  - Verify resource existence and configuration in Azure Portal.
  - Check storage account access, private endpoint, and DNS zone linkage.
- **Validation:** All resources are present, private endpoint and DNS are functional, and public access is restricted.

**Exercise 5: Stretch Goals (Advanced Scenarios)**
- **Goal:** Enhance infrastructure with tags, dynamic subnet addressing, and diagnostics.
- **Actions:**
  - Add tags to all resources and resource group via variables and module inputs.
  - Use AVM utility module to calculate subnet prefix CIDR dynamically.
  - Add Log Analytics Workspace and configure diagnostic settings for all resources using locals.
  - Format, plan, apply, and validate changes; commit after each enhancement.
- **Validation:** Tags and diagnostics are visible in Azure Portal; subnet addressing is dynamic and correct.

**Exercise 6: Cleanup**
- **Goal:** Remove all deployed resources to avoid unnecessary costs.
- **Actions:**
  - Run Terraform destroy plan and apply to delete all resources.
- **Validation:** Azure resources are deleted and environment is clean.

**Exercise 7: Lab Completion**
- **Goal:** Complete the lab and submit for credit.
- **Actions:**
  - Answer survey questions and select End to mark the lab as complete.
- **Validation:** Lab completion is recorded and feedback is submitted.
