---
title: 'Build your own pizza ordering agent - Ignite 2025'
layout: default
nav_order: 10
parent: 'Lab summaries'
---

**ID** 205048
**Number:** LAB571
**Name:** Build your own pizza ordering agent - Ignite 2025
**CloudSubscriptionPoolName:** Microsoft Events 25 - MSLEARN CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Create Your First Agent**
- **Goal:** Build a basic AI agent using Foundry Agent Service and interact with it locally.
- **Actions:**
  - Log into Azure and set up the development environment in VS Code.
  - Create a .env file with the Foundry project connection string.
  - Write a Python script to instantiate an agent using the GPT-4o model.
  - Implement a conversation loop to interact with the agent and clean up resources after use.
- **Validation:**
  - Successfully run the agent script and receive responses in the terminal.

**Exercise 2: Adding Agent Instructions**
- **Goal:** Customize agent behavior using system prompts and external instruction files.
- **Actions:**
  - Create an instructions.txt file with detailed agent guidelines.
  - Update the agent creation code to load instructions from the file and set generation parameters (top_p, temperature).
- **Validation:**
  - Observe agent responses reflecting the custom instructions and settings.

**Exercise 3: Adding Knowledge with File Search (RAG)**
- **Goal:** Enable the agent to answer questions using custom data via Retrieval-Augmented Generation.
- **Actions:**
  - Write a script to upload documents, create a vector store, and vectorize files for search.
  - Integrate a File Search tool and toolset into the agent.
- **Validation:**
  - Agent accurately answers questions using uploaded Contoso Pizza store data.

**Exercise 4: Tool Calling - Pizza Calculator**
- **Goal:** Extend the agent with a custom tool for pizza size recommendations.
- **Actions:**
  - Implement a pizza calculator function in tools.py.
  - Register the function as a FunctionTool and add it to the agent's toolset.
  - Enable automatic function calling for the toolset.
- **Validation:**
  - Agent provides pizza recommendations based on group size and appetite when prompted.

**Exercise 5: Integrating MCP (Model Context Protocol)**
- **Goal:** Connect the agent to a live MCP server for real-time menu and order management.
- **Actions:**
  - Add and configure an MCP tool for Contoso Pizza microservices.
  - Implement a custom run handler for tool approval.
  - Update instructions with user details and test live order scenarios.
- **Validation:**
  - Agent can retrieve menus, place orders, and interact with live services via MCP tools.
