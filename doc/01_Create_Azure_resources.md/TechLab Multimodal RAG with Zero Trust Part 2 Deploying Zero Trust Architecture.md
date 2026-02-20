---
title: 'TechLab: Multimodal RAG with Zero Trust Part 2: Deploying Zero Trust Architecture'
layout: default
nav_order: 77
parent: 'Lab summaries'
---

**ID** 183563  
**Number:** 1  
**Name:** TechLab: Multimodal RAG with Zero Trust Part 2: Deploying Zero Trust Architecture  
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)  
**AllowSave:** True  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Zero Trust Architecture Review**
- **Goal:** Understand and analyze the Zero Trust Architecture (ZTA) applied to GPT-RAG deployments in Azure.
- **Actions:**
  - Review the architecture diagram focusing on VNets, Private Endpoints, and resource group components.
  - Identify and understand the role of key Azure resources: VNets, Private Endpoints, App Service Plan, Data Science VM, Key Vault, and RBAC.
  - Examine authentication and authorization flows using Azure Entra ID and MSAL.
  - Summarize the security and operational benefits of Zero Trust in the deployment.
- **Validation:** Architecture components and security controls are clearly identified and mapped to Zero Trust principles.

**Exercise 2: Application Deployment**
- **Goal:** Deploy GPT-RAG application components in a Zero Trust environment using Azure Bastion and private networking.
- **Actions:**
  - Monitor and verify resource provisioning with network isolation enabled (AZURE_NETWORK_ISOLATION=true).
  - Connect to a VM via Azure Bastion and install required tools (PowerShell 7, azd).
  - Initialize and deploy the GPT-RAG environment from within the private network, authenticating with Azure credentials.
- **Validation:** All required Azure resources are provisioned, and deployment completes successfully within the isolated network.

**Exercise 3: Test/Validate Networking Configuration**
- **Goal:** Validate that Zero Trust network controls are enforced for all key application endpoints.
- **Actions:**
  - Attempt to access the frontend app, orchestrator endpoint, and blob storage from a public network to confirm access is blocked (403 errors).
  - Access the same resources from the internal Bastion VM to confirm access is allowed for trusted network zones.
- **Validation:** Public access is denied and internal access is permitted, demonstrating effective Zero Trust enforcement for all critical endpoints.
