---
title: 'Building collaborative agents in Microsoft Teams with Teams AI Library'
layout: default
nav_order: 12
parent: 'Lab summaries'
---

**ID** 205920  
**Number:** LAB590  
**Name:** Building collaborative agents in Microsoft Teams with Teams AI Library  
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** M365Copilot, E5, TeamsEnt  

---

## Exercise Summary

**Exercise 1: Build Your Agent in 30 Seconds**
- **Goal:** Quickly create a basic Teams agent using the Teams CLI.
- **Actions:**
  - Install Teams CLI and scaffold a new echo agent project in TypeScript.
  - Install dependencies and run the development server.
  - Test the agent using DevTools and verify echo functionality.
- **Validation:**
  - Agent responds to messages in DevTools by echoing input.

**Exercise 2: Explore DevTools**
- **Goal:** Learn to use Teams DevTools for agent testing and debugging.
- **Actions:**
  - Interact with the agent in DevTools (send, edit, delete messages; inspect activities).
  - Review activity payloads and connectivity status.
- **Validation:**
  - Successful message interactions and activity inspection in DevTools.

**Exercise 3: Setting Up AI Resources on Microsoft Foundry**
- **Goal:** Deploy and configure AI resources for agent intelligence.
- **Actions:**
  - Create a Microsoft Foundry resource and deploy the gpt-4o model.
  - Launch Teams in Edge and sign in with provided credentials.
- **Validation:**
  - Foundry resource and model are deployed and accessible; Teams is ready for agent integration.

**Exercise 4: Connect Tech Support Agent to Microsoft Foundry Resources**
- **Goal:** Integrate the agent with M365 Agents Toolkit and Foundry AI model.
- **Actions:**
  - Use the M365 Agents Toolkit to create a new Teams agent project.
  - Configure the agent with Foundry API key, endpoint, and gpt-4o model.
  - Replace source code with provided Tech Support Agent code and run/debug in Teams.
  - Interact with the agent using adaptive cards and submit a laptop request.
- **Validation:**
  - Agent responds in Teams, processes tech support requests, and displays adaptive cards.

**Exercise 5: Add Advanced Orchestration (via the Model Context Protocol)**
- **Goal:** Enable the agent to act as an MCP client for order approval workflows.
- **Actions:**
  - Install the MCP Client package and update agent code to use MCP client plugin.
  - Configure MCP server URL and API key in the agent.
  - Run/debug the agent and submit order approval requests.
  - Review logs to confirm MCP tool usage and responses.
- **Validation:**
  - Agent successfully calls MCP server, receives approval/denial, and logs MCP activity.
