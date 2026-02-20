---
title: 'TechLab: Extend Microsoft 365 copilot with declarative agent using M365'
layout: default
nav_order: 68
parent: 'Lab summaries'
---

**ID** 200795  
**Number:** 1  
**Name:** TechLab: Extend Microsoft 365 copilot with declarative agent using M365  
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** M365Copilot, CopilotStudio, E3  

---

## Exercise Summary

**Exercise 1: Build a Backend API for the Solution**
- **Goal:** Set up and test a TypeScript-based Azure Functions REST API for a consulting scenario, using local emulated Azure Table Storage.
- **Actions:**
  - Download and extract the starter project, open it in VS Code, and configure environment files.
  - Install dependencies and sign in to the Microsoft 365 Agents Toolkit.
  - Set up a persistent developer tunnel and update project configuration for stable API URLs.
  - Start the local API, test endpoints using the provided .http file, and review data in the Azurite emulator.
- **Validation:**
  - API endpoints return expected data for test requests.
  - Data is visible and modifiable in the local storage emulator.

**Exercise 2: Build a Declarative Agent Grounded with API and SharePoint Files**
- **Goal:** Create a Microsoft 365 declarative agent that integrates the custom API and SharePoint files, and test its functionality in Copilot chat.
- **Actions:**
  - Analyze the provided SharePoint site and add its URL to the agent configuration.
  - Create a declarative agent JSON file referencing the API plugin and SharePoint capability.
  - Review and understand the OpenAPI and plugin manifest files for the API.
  - Update the app manifest to register the declarative agent and remove unnecessary features.
  - Increment the manifest version and ensure all configuration is correct.
  - Run and debug the agent, test prompts in Copilot chat, and review API calls and adaptive card responses.
- **Validation:**
  - Declarative agent responds to prompts, accesses API and SharePoint data, and displays results with citations and adaptive cards in Copilot chat.
  - API calls are logged and responses are visible in the chat interface.
