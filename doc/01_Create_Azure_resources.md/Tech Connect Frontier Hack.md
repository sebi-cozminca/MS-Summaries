---
title: 'Tech Connect Frontier Hack'
layout: default
nav_order: 49
parent: 'Lab summaries'
---

**ID** 209295  
**Number:** HYB 787  
**Name:** Tech Connect Frontier Hack  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** CopilotStudio, E3, Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Lab Environment Setup**
- **Goal:** Prepare the virtual machine and access required credentials for the lab.
- **Actions:**
  - Sign in to the provided virtual machine using lab credentials.
  - Access the Resources tab to retrieve Microsoft 365 and Azure credentials for use throughout the lab.
- **Validation:**
  - Successful login to the VM and access to all required credentials.

**Exercise 2: Zone 1 – Build a Retrieval Agent (Copilot Chat)**
- **Goal:** Create a trustworthy retrieval-based agent grounded in business data using Microsoft 365 Copilot.
- **Actions:**
  - Review the provided CRM_Synthetic_Data.xlsx dataset for structure and gaps.
  - Use Microsoft 365 Copilot to create a new agent, provide clear instructions, and upload the dataset as knowledge.
  - Test the agent with realistic portfolio-level questions and refine instructions as needed.
- **Validation:**
  - Agent is accessible, grounded in the dataset, answers at least three realistic questions, and does not fabricate answers when data is missing.

**Exercise 3: Zone 2 – Build a Reasoning & Routing Agent (Copilot Studio)**
- **Goal:** Develop an agent in Copilot Studio that analyzes user intent and routes conversations to appropriate topic flows.
- **Actions:**
  - Create a new agent in Copilot Studio, attach the CRM dataset, and configure agent instructions.
  - Build a central intent analysis topic and child topics for different response styles (e.g., summary, details).
  - Use AI Prompt Builder for intent classification and configure routing logic.
  - Add generative answers to topics and test the conversation flow.
  - Optionally, extend the agent with orchestration or richer reasoning as a challenge.
- **Validation:**
  - Agent includes a central intent analysis topic, routes requests to at least two topic paths, responses are data-grounded, and conversation paths end cleanly. Optional: agent can take actions with user confirmation.

**Exercise 4: Zone 3 – Design & Orchestrate an Agent System (Azure AI Foundry)**
- **Goal:** Design and orchestrate a multi-agent system using Azure AI Foundry, focusing on system-level design and workflow.
- **Actions:**
  - Create a new project in Azure AI Foundry, deploy a model, and create a retrieval-based agent using the provided CRM JSON data.
  - Build a workflow to orchestrate agent behavior and test agent interactions.
  - Optionally, use Visual Studio Code with the Azure AI Foundry extension for further exploration.
  - As a group, design an agent system for a real-world scenario, extending or modifying agents and workflows as needed.
- **Validation:**
  - System clearly states the real-world scenario, uses sample data, demonstrates at least one grounded agent interaction, includes a workflow/orchestration step, and explains how the design could extend to real data or systems. Optional: multiple agents, intent-based routing, structured outputs, and dynamic data grounding.
