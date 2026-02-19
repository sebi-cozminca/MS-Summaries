---
title: 'Building Powerful Agents with Microsoft 365 Agent SDK'
layout: default
nav_order: 16
parent: 'Lab summaries'
---

**ID** 202169
**Number:** LAB 483
**Name:** Building Powerful Agents with Microsoft 365 Agent SDK
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** M365Copilot, E3, TeamsEnt

---

# Building Powerful Agents with Microsoft 365 Agent SDK — Lab Instruction Summary

## Exercise Summary

**Exercise 1: Prerequisites and Environment Setup**
- **Goal:** Prepare the environment and required services for agent development with Microsoft 365 Agent SDK.
- **Actions:**
  - Set up Microsoft Teams for custom app uploads.
  - Install Visual Studio Code, .NET SDK, C# Dev Kit, Microsoft 365 Agents Toolkit, Azure CLI, and DevTunnel.
  - Create a Microsoft Foundry project, deploy the gpt-4.1 model, and configure content safety filters.
  - Save Azure OpenAI endpoint, API key, and deployment name for later use.
- **Validation:**
  - All tools and services are installed and configured; credentials and endpoints are available for agent integration.

**Exercise 2: Build and Run Your First Agent**
- **Goal:** Build, configure, and launch a basic insurance claims agent using the Microsoft 365 Agent SDK and Agents Framework.
- **Actions:**
  - Clone the starter repository and explore the project structure (Agent, Plugins, app manifest, environment files).
  - Configure environment files with Azure AI credentials and sign in to Microsoft 365 and Azure.
  - Provision Azure resources and run the agent locally using Visual Studio Code.
  - Test agent responses in Microsoft 365 Copilot, including conversation starters and plugin calls.
  - Personalize the agent by updating the welcome message.
- **Validation:**
  - Agent runs successfully, responds to test queries in Copilot, and displays personalized welcome messages.

**Exercise 3: Add Document Search with Azure AI Search**
- **Goal:** Enhance the agent with AI-powered claims search and retrieval using Azure AI Search and OpenAI.
- **Actions:**
  - Create and configure an Azure AI Search service and deploy an embedding model.
  - Add sample claims data and update environment files with search credentials.
  - Implement the KnowledgeBaseService for search, indexing, and retrieval.
  - Build the ClaimsPlugin to expose claim search and detail retrieval tools.
  - Register services and plugins in Program.cs and agent configuration.
  - Update the agent's instructions and welcome message to reflect new capabilities.
  - Run and test the agent, verifying claims search and detail retrieval in Copilot and Azure Portal.
- **Validation:**
  - Agent returns accurate claim search results and details; Azure AI Search index and knowledge base are populated and accessible; successful test queries in Copilot and Azure Portal.
