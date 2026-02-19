---
title: 'TechLab: Designing your own Agent with Copilot Studio'
layout: default
nav_order: 63
parent: 'Lab summaries'
---

**ID** 185898
**Number:** 45-404-36
**Name:** TechLab: Designing your own Agent with Copilot Studio
**CloudSubscriptionPoolName:** NA
**AllowSave:** True
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise Blank Admin Only 15S (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

### Exercise Summary

**Exercise 00: Setup**
- **Goal:** Set up Copilot Studio environment and import a pre-built agent for lab use.
- **Actions:**
  - Sign in to Copilot Studio, start a free trial, and switch to the correct environment.
  - Import a pre-built agent solution for use in subsequent exercises.
- **Validation:**
  - Copilot Studio is accessible in the correct environment; pre-built agent appears in the Agents list.

**Exercise 01: Explore the agent in Microsoft Copilot Studio**
- **Goal:** Learn Copilot Studio agent structure and authoring basics by creating, editing, and testing agents and topics.
- **Actions:**
  - Create a new agent using natural language prompts.
  - Test the pre-built agent and explore conversation flow using the test pane.
  - Edit topic triggers, questions, messages, and conditions; use Copilot to generate and modify topics.
  - Publish the agent to a demo website and test live interactions.
- **Validation:**
  - Agent responds to test prompts; topic edits are reflected in agent behavior and demo website.

**Exercise 02: Authoring 101**
- **Goal:** Understand entities, topic logic, message formatting, and Power Fx for dynamic agent conversations.
- **Actions:**
  - Explore closed list and regex entities and observe their use in Question nodes.
  - Review topic management nodes for conversation flow control and reusable topics.
  - Enhance messages with rich text, images, quick replies, and message variations.
  - Use the YAML code editor and Power Fx for advanced customization and variable formatting.
- **Validation:**
  - Entities extract user input as expected; message formatting and logic changes are visible in agent responses.

**Exercise 03: Build and call Power Automate cloud flows from your agent**
- **Goal:** Integrate Power Automate flows to extend agent capabilities with external data and automation.
- **Actions:**
  - Explore Action nodes that call Power Automate flows and pass topic variables.
  - Parse JSON output from flows and display results using Adaptive Cards and Power Fx.
- **Validation:**
  - Agent retrieves and displays external data (e.g., ticket status) in formatted responses after flow execution.

**Exercise 04: Make HTTP requests to connect to an API**
- **Goal:** Enable the agent to call external APIs using HTTP Request nodes and dynamic Power Fx URLs.
- **Actions:**
  - Configure HTTP Request nodes to call external APIs (e.g., Gemini API for Bitcoin prices).
  - Use Power Fx to construct request URLs based on user input and display API results in the conversation.
- **Validation:**
  - Agent successfully fetches and presents external API data in response to user queries.
