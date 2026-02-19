---
title: 'TechLab: Build Scalable AI Apps with AKS & APIM'
layout: default
nav_order: 55
parent: 'Lab summaries'
---

**ID** 169588
**Number:** 41-411-10
**Name:** TechLab: Build Scalable AI Apps with AKS & APIM
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** E5

---

# Tech Mastery Catalog Lab Instruction Summary

## Exercise Summary

**Exercise 0: Provision Azure Services**
- **Goal:** Set up all required Azure infrastructure for scalable AI app deployment.
- **Actions:**
  - Select Azure regions for resource deployment.
  - Create Application Insights and Log Analytics workspace.
  - Provision API Management (APIM) with managed identity.
  - Deploy two Azure OpenAI instances (in different regions) and deploy GPT-4o model to each.
  - Provision an AKS cluster for app hosting.
- **Validation:** All resources are visible in the Azure portal and configured in the correct regions.

**Exercise 1: Review and Verify Deployed Resources**
- **Goal:** Confirm all Azure resources are operational and ready for use.
- **Actions:**
  - Verify presence of all required resources in the resource group.
  - Test GPT-4o deployments in both OpenAI instances using Azure AI Foundry portal.
  - Check AKS cluster node status.
  - Confirm APIM service is online.
- **Validation:** Successful test prompts return expected responses; AKS nodes are running; APIM status is "Online".

**Exercise 2: Deploy and Test the AKS Store Demo App**
- **Goal:** Deploy the AKS Store Demo app and supporting microservice, then validate end-to-end functionality.
- **Actions:**
  - Deploy the AKS Store app to the AKS cluster using kubectl in Azure Cloud Shell.
  - Download, configure, and deploy a Python-based microservice for Azure OpenAI integration.
  - Test the Store app by adding a product and using the AI assistant for product description generation.
- **Validation:** Store app is accessible; AI assistant generates product descriptions; microservice and pods are running.

**Exercise 3: Configure APIM**
- **Goal:** Set up APIM to load balance requests across multiple Azure OpenAI instances.
- **Actions:**
  - Assign APIM managed identity to both OpenAI instances.
  - Create APIM backends for each OpenAI instance and a pool backend using REST API calls.
  - Import Azure OpenAI API specification from GitHub and configure in APIM.
  - Add inbound policy for authentication and metrics.
  - Create a subscription in APIM and retrieve keys and gateway URL.
  - Test the API via APIM and review transaction data in Application Insights.
- **Validation:** APIM routes requests to OpenAI instances; API tests return valid responses; metrics and transaction data are visible in Application Insights.

**Exercise 4: Update and Test the Solution**
- **Goal:** Reconfigure the microservice to use APIM as the unified endpoint and validate multi-instance AI integration.
- **Actions:**
  - Update ai-service.yaml to use APIM gateway URL and subscription key.
  - Redeploy the updated microservice to the AKS cluster.
  - Test the Store app to ensure product descriptions are generated via APIM.
- **Validation:** Store app successfully uses APIM for AI-powered product descriptions; microservice operates as expected after reconfiguration.
