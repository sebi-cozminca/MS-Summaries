---
title: 'Build and deploy AI Agents with MCP and Azure Functions - Ignite 2025'
layout: default
nav_order: 8
parent: 'Lab summaries'
---

**ID** 205279
**Number:** LAB514
**Name:** Build and deploy AI Agents with MCP and Azure Functions - Ignite 2025
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

### Exercise Summary

**Lab Setup**
- **Goal:** Prepare the lab environment and required tools for building and deploying AI agents with Azure Functions and MCP.
- **Actions:**
  - Log in to the Windows 11 lab VM and opt out of backup prompts.
  - Open Edge with pre-configured tabs for the Snippy GitHub repo, Azure Portal, and Microsoft Foundry.
  - Clone the Snippy repository, launch VS Code, and sign in to GitHub Copilot with provided credentials.
- **Validation:**
  - All required tools are accessible, and the Snippy repo is open in VS Code with Copilot enabled.

**Resource Provisioning and Local Setup**
- **Goal:** Provision Azure resources and configure the local development environment for Snippy.
- **Actions:**
  - Use Azure Developer CLI (azd) to authenticate, create an environment, and provision resources (Function App, Cosmos DB, Azure AI, etc.).
  - Install Python dependencies, verify local.settings.json, and start Docker Compose for Durable Task support.
- **Validation:**
  - Resources are provisioned, local settings are populated, and Docker containers for Durable Task and Azurite are running.

**Code Review and Implementation Patterns**
- **Goal:** Understand and review how Azure Functions integrate with MCP and AI agents.
- **Actions:**
  - Review tool schema definitions, MCP tool trigger bindings, and embeddings input bindings in function_app.py.
  - Examine durable agent definitions and orchestration patterns in durable_agents.py.
  - Review the vector_search tool for semantic retrieval in tools/vector_search.py.
- **Validation:**
  - Code implements MCP tool registration, automated embedding generation, and agent orchestration as described.

**Local Testing and MCP Integration**
- **Goal:** Test the application locally and validate MCP tool integration with GitHub Copilot.
- **Actions:**
  - Start the Azure Functions runtime locally and test endpoints using REST Client.
  - Connect Copilot Chat to the local MCP server, test saving and retrieving snippets, and use agent-based tools (deep_wiki, code_style).
  - Monitor function logs and Durable Task Scheduler UI for orchestration progress.
- **Validation:**
  - All tools and agent orchestrations work as expected locally, with successful end-to-end tests and visible logs.

**Cloud Deployment and Monitoring**
- **Goal:** Deploy the application to Azure and validate cloud-based MCP and agent orchestration.
- **Actions:**
  - Deploy the code to Azure using azd deploy, configure VS Code/Copilot to use the cloud MCP endpoint, and test tool usage in the cloud.
  - Monitor orchestrations in the Durable Task Scheduler dashboard and review generated documentation files.
- **Validation:**
  - Cloud-hosted MCP tools and agent orchestrations function correctly, with successful monitoring and output verification.

**Clean-up**
- **Goal:** Remove all lab resources and sign out of accounts to prevent unnecessary charges or access.
- **Actions:**
  - Run azd down --purge --force to delete Azure resources and local environment configuration.
  - Sign out of GitHub and all accounts in Microsoft Edge.
- **Validation:**
  - All resources are deleted and accounts are signed out, completing the lab clean-up process.
