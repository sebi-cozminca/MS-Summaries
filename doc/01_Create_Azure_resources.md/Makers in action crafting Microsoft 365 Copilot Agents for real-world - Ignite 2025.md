---
title: 'Makers in action: crafting Microsoft 365 Copilot Agents for real-world - Ignite 2025'
layout: default
nav_order: 36
parent: 'Lab summaries'
---

**ID** 205063  
**Number:** LAB565  
**Name:** Makers in action: crafting Microsoft 365 Copilot Agents for real-world - Ignite 2025  
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** Events GHE w/ Copilot, M365Copilot, CopilotStudio, E3  

---

## Exercise Summary

**Exercise 1: Setting up the MCP Server**
- **Goal:** Deploy and run a local MCP server for HR candidate management.
- **Actions:**
  - Review project structure and key files (configuration, data, services, tools, entry point).
  - Build and run the .NET MCP server locally using `dotnet run`.
  - Expose the local server via Microsoft dev tunnel for public access.
  - Test server connectivity using MCP Inspector.
- **Validation:**
  - MCP server responds at localhost and via dev tunnel URL.
  - MCP Inspector successfully connects and lists available tools.

**Exercise 2: Creating a New Agent in Copilot Studio**
- **Goal:** Create a Copilot Studio agent to consume the MCP server.
- **Actions:**
  - Activate Copilot Studio license and access the platform.
  - Create a new agent with specified name, description, and instructions.
  - Configure suggested prompts for common candidate management tasks.
- **Validation:**
  - Agent is created and prompts are available in Copilot Studio.

**Exercise 3: Integrating MCP Server with Copilot Studio**
- **Goal:** Connect the Copilot Studio agent to the MCP server and enable tool usage.
- **Actions:**
  - Add the MCP server as a tool in the agent's configuration.
  - Establish a connection to the MCP server (using dev tunnel URL, no auth).
  - Publish the agent and test tool invocation (e.g., list candidates).
- **Validation:**
  - Agent successfully invokes MCP server tools and returns candidate data.

**Exercise 4: Creating and Populating the Search Index**
- **Goal:** Set up Azure AI Search with vectorized candidate resumes for RAG.
- **Actions:**
  - Review and upload sample resume PDFs to Azure Storage Account.
  - Use Azure AI Search to import, vectorize, and index documents (using OpenAI embeddings).
  - Save service endpoint and admin key for later use.
- **Validation:**
  - Azure AI Search index is created and populated; search returns indexed documents.

**Exercise 5: Creating the RAG-Enabled Agent**
- **Goal:** Enhance the Copilot Studio agent with Azure AI Search for RAG.
- **Actions:**
  - Update agent instructions to leverage vector search and document-backed responses.
  - Disable MCP server tool; add Azure AI Search as a knowledge source.
  - Configure connection using endpoint and admin key; select the resumes index.
- **Validation:**
  - Knowledge source status is "Ready" in Copilot Studio.

**Exercise 6: Testing the Agent**
- **Goal:** Validate agent's ability to answer queries using RAG and Azure AI Search.
- **Actions:**
  - Test basic and advanced queries in Copilot Studio's test panel.
  - Observe semantic search, citations, and candidate recommendations.
- **Validation:**
  - Agent provides relevant, cited responses based on indexed resumes and search criteria.
