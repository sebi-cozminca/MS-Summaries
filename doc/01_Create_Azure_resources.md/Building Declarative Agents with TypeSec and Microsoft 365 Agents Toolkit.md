---
title: 'Building Declarative Agents with TypeSec and Microsoft 365 Agents Toolkit'
layout: default
nav_order: 14
parent: 'Lab summaries'
---

**ID** 207426
**Number:** LAB 485
**Name:** Building Declarative Agents with TypeSec and Microsoft 365 Agents Toolkit
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** M365Copilot, CopilotStudio, E3

---

# Exercise Summary

**Exercise 1: Connect Declarative Agent to MCP Server**
- **Goal:** Integrate a Declarative Agent with an MCP server to enable natural language access to insurance claims data.
- **Actions:**
  - Test the hosted MCP server using the MCP Inspector and verify available tools.
  - Create a new Declarative Agent project with Microsoft 365 Agents Toolkit, connecting it to the MCP server and selecting relevant tools.
  - Configure agent identity, instructions, and conversation starters for claims operations.
  - Update the Teams app manifest for branding and permissions.
  - Provision and test the agent in Microsoft 365 Copilot, verifying claims data access and debugging as needed.
- **Validation:**
  - Agent responds to natural language queries, retrieves and manages claims data, and MCP server integration is confirmed in Copilot chat.

**Exercise 2: Multi-Agent Claims Orchestration**
- **Goal:** Build a multi-agent orchestration solution by connecting specialized Declarative Agents for claims and procurement.
- **Actions:**
  - Create a new Declarative Agent for procurement, embedding contractor pricing and guidelines as local knowledge files.
  - Configure agent identity, instructions, and manifest for procurement tasks.
  - Provision and test the procurement agent in Microsoft 365 Copilot, verifying access to embedded knowledge.
  - Create an orchestrator agent (ZavaCare) and connect it to both claims and procurement agents using their IDs.
  - Configure orchestrator agent instructions for workflow coordination and multi-agent responses.
  - Provision and test the orchestrator agent, validating multi-agent workflows and coordinated responses.
- **Validation:**
  - Orchestrator agent successfully coordinates between claims and procurement agents, providing unified responses to complex queries in Copilot chat.
