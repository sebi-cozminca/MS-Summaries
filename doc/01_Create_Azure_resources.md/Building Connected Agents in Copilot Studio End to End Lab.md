---
title: 'Building Connected Agents in Copilot Studio: End to End Lab'
layout: default
nav_order: 13
parent: 'Lab summaries'
---

**ID** 208653
**Number:** LAB 633
**Name:** Building Connected Agents in Copilot Studio: End to End Lab
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** CopilotStudio, Events GHE w/ Copilot, E3 + PBI Pro

---

# Exercise Summary

**Exercise 1: Create and Configure Fabric Data Agent**
- **Goal:** Build a Fabric Data Agent that can query a semantic model using natural language.
- **Actions:**
  - Create a new Microsoft Fabric workspace and Lakehouse.
  - Import the Retail sample dataset and verify tables.
  - Create a semantic model from Lakehouse tables, add relationships and measures, and publish the model.
  - Create a Fabric Data Agent, connect it to the semantic model, and test with baseline queries.
  - Use meta-prompts to generate and refine agent instructions for optimal performance.
- **Validation:**
  - Agent returns accurate, data-backed answers to test queries and displays generated DAX; instructions are optimized and published.

**Exercise 2: Connect Fabric Data Agent to Copilot Studio**
- **Goal:** Enable agent-to-agent communication by connecting the Fabric Data Agent to Copilot Studio as a connected agent.
- **Actions:**
  - Create a new Copilot Studio agent and configure its name, description, and instructions.
  - Set the model (e.g., Claude Sonnet 4.5) and optionally enable deep reasoning.
  - Add the Fabric Data Agent as a connected agent (MCP server), configure credentials, and finalize the connection.
  - Test the integrated solution with queries of increasing complexity, verifying delegation and data agent responses.
- **Validation:**
  - Copilot Studio agent successfully delegates queries to the Fabric Data Agent, which returns structured analytics and insights.

**Optional Challenge Activities**
- **Goal:** Extend and optimize the connected agent ecosystem.
- **Actions:**
  - Create additional Fabric Data Agents for other domains and connect them to Copilot Studio.
  - Enable code interpreter for visualizations, develop advanced meta-prompts, and upload additional knowledge sources.
  - Experiment with model selection and performance tuning.
- **Validation:**
  - Multi-agent orchestration, visual outputs, and enhanced contextual reasoning are demonstrated in test scenarios.