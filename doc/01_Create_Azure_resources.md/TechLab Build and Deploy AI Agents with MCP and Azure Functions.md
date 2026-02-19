---
title: 'TechLab: Build and Deploy AI Agents with MCP and Azure Functions'
layout: default
nav_order: 54
parent: 'Lab summaries'
---

**ID** 186838
**Number:** LAB344
**Name:** TechLab: Build and Deploy AI Agents with MCP and Azure Functions
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Tech Mastery Catalog Lab Instruction Summary

## Exercise Summary

**Exercise 1: Lab Set-up**
- **Goal:** Prepare the lab environment with all required tools and access.
- **Actions:**
  - Log in to the Windows 11 lab VM.
  - Open Edge with pre-configured tabs for GitHub, Azure Portal, and Azure AI Foundry.
  - Review available software (VS Code, Python, uv, Azure CLI, Azure Functions Core Tools, AZD).
- **Validation:** Successful login to VM and access to all required tools and browser tabs.

**Exercise 2: Fork the Repository**
- **Goal:** Create a personal fork of the Snippy lab repository for development.
- **Actions:**
  - Fork the GitHub repository from the provided link.
  - Ensure the correct branch (build-2025) is available.
  - Validate the forked repository URL.
- **Validation:** Forked repository is accessible and correct branch is checked out.

**Exercise 3: Clone the Repo and Set Up in VS Code**
- **Goal:** Clone the forked repository and prepare the codebase for editing.
- **Actions:**
  - Clone the forked repo using Git in the terminal.
  - Check out the build-2025 branch and fetch the bonus branch.
  - Open the project in VS Code.
  - Edit infra/main.bicep to update resource naming and group definitions.
- **Validation:** Project opens in VS Code with correct branch and updated configuration.

**Exercise 4: Sign in to GitHub Copilot**
- **Goal:** Enable GitHub Copilot integration in VS Code.
- **Actions:**
  - Sign in to GitHub Copilot via VS Code.
  - (Optional) Sign in to Azure in VS Code for resource management.
- **Validation:** Copilot is signed in and available in VS Code.

**Exercise 5: Start Resource Provisioning with AZD**
- **Goal:** Provision all required Azure resources for the Snippy application.
- **Actions:**
  - Log in to Azure using azd auth login.
  - Create a new azd environment.
  - Run azd provision to deploy infrastructure (Function App, Cosmos DB, AI services, Key Vault, etc.).
- **Validation:** azd provision completes successfully and resources are visible in Azure Portal.

**Exercise 6: Coding Exercises – Implement MCP Tools and AI Agents**
- **Goal:** Build and enhance Azure Functions for AI-powered code snippet management and agent orchestration.
- **Actions:**
  - Define tool properties for save_snippet in function_app.py.
  - Add MCP Tool Trigger decorator to expose function as an MCP tool.
  - Add embeddings input binding for automatic vector embedding generation.
  - Review deep_wiki agent orchestration code for agent creation and tool integration.
  - Explore RAG pattern and vector search in Cosmos DB.
- **Validation:** Code changes are implemented; functions are ready for local testing.

**Exercise 7: Local Setup – Install Python Dependencies**
- **Goal:** Prepare the Python environment for local development and testing.
- **Actions:**
  - Navigate to src directory.
  - Create and activate a Python virtual environment using uv.
  - Install dependencies from requirements.txt.
- **Validation:** All dependencies are installed and environment is activated.

**Exercise 8: Verify Local Settings After Provisioning**
- **Goal:** Ensure local.settings.json is correctly populated for local execution.
- **Actions:**
  - Check or regenerate local.settings.json with correct resource values.
- **Validation:** local.settings.json contains all required settings for local execution.

**Exercise 9: Run Functions Locally and Test with Cloud Resources**
- **Goal:** Test the Azure Functions locally against provisioned cloud resources.
- **Actions:**
  - Start the Azure Functions runtime locally.
  - Use REST Client to test endpoints (save, retrieve, and agent-based functions).
  - Connect Copilot Chat to local MCP endpoint and test tool integration.
- **Validation:** Functions respond correctly to HTTP and MCP tool requests; logs confirm successful execution.

**Exercise 10: Deploy the Application Code to Azure**
- **Goal:** Deploy the completed application to the Azure Function App.
- **Actions:**
  - Stop local host, navigate to project root, and run azd deploy.
- **Validation:** Deployment completes and endpoints are available in Azure.

**Exercise 11: Connect VS Code / Copilot to the Cloud MCP Endpoint**
- **Goal:** Enable Copilot and VS Code to use the deployed cloud MCP tools.
- **Actions:**
  - Authenticate with Azure CLI and retrieve the MCP system key.
  - Configure .vscode/mcp.json for the cloud endpoint.
  - Test tool usage in Copilot Chat against the deployed cloud endpoint.
- **Validation:** Copilot can invoke deployed MCP tools and receive correct responses.

**Exercise 12: Clean-up**
- **Goal:** Remove all provisioned resources and sign out of accounts.
- **Actions:**
  - Run azd down --purge --force to delete Azure resources.
  - Sign out of GitHub and Azure accounts.
- **Validation:** All resources are deleted and accounts are signed out.
