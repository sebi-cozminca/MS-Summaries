---
title: 'TechLab: Azure landing zone + AI-Ready Landing Zone Accelerator for AI'
layout: default
nav_order: 53
parent: 'Lab summaries'
---

**ID** 187932  
**Number:** LAB618  
**Name:** TechLab: Azure landing zone + AI-Ready Landing Zone Accelerator for AI  
**CloudSubscriptionPoolName:** Build 2024 CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise Blank Admin Only 15S (Stakeholder: Kim Frank)  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Deploy the Infrastructure**
- **Goal:** Provision a secure, AI-ready Azure landing zone with all required networking, security, and AI service dependencies.
- **Actions:**
  - Sign in to the lab VM and Azure portal with provided credentials.
  - Use Azure Cloud Shell to clone the reference repository and set up environment variables.
  - Generate and encode TLS certificates for Application Gateway.
  - Set deployment location and base resource names.
  - Deploy infrastructure using Bicep templates, including network, storage, AI services, and security resources.
- **Validation:**
  - Resource group and all required resources are deployed and visible in the Azure portal; deployment completes without errors.

**Exercise 2: Deploy an Agent in the Azure AI Agent Service**
- **Goal:** Deploy a GPT-based AI agent with Bing grounding in Azure AI Foundry, simulating a CI/CD pipeline deployment.
- **Actions:**
  - Connect to the jump box VM via Bastion and sign in to Azure.
  - Set environment variables and download the agent definition.
  - Update agent configuration and deploy the agent using Azure CLI and REST API.
  - Capture the deployed agent's ID for later use.
- **Validation:**
  - Agent is deployed and listed in the Azure AI Foundry project; agent ID is available for integration.

**Exercise 3: Test the Agent from the Azure AI Foundry Portal**
- **Goal:** Validate agent orchestration and grounding by interacting with the agent in the Azure AI Foundry playground.
- **Actions:**
  - Access the Azure AI Foundry portal from the jump box VM.
  - Locate the deployed agent and use the playground to submit queries requiring Bing-grounded responses.
- **Validation:**
  - Agent returns grounded, generative responses to test queries in the playground interface.

**Exercise 4: Publish the Chat Front-End Web App**
- **Goal:** Deploy and configure a chat UI web application to interact with the Azure AI Agent service.
- **Actions:**
  - Download the chat UI package and upload it to Azure Storage.
  - Update App Service configuration to use the deployed agent ID.
  - Restart the web app to apply changes.
- **Validation:**
  - Web app is updated and configured to communicate with the deployed agent.

**Exercise 5: Test the Deployed Application End-to-End**
- **Goal:** Validate the full application stack, including networking, web app, and agent orchestration.
- **Actions:**
  - Retrieve the Application Gateway public IP and update the local hosts file for DNS resolution.
  - Access the chat UI via browser and submit queries that require Bing-based grounding.
- **Validation:**
  - Application is accessible via the configured domain; chat queries return grounded, generative responses from the agent.
