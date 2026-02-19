---
title: 'Building intelligent, multi-agent Apps with Github and Agent Framework'
layout: default
nav_order: 15
parent: 'Lab summaries'
---

**ID** 208623
**Number:** LAB 181
**Name:** Building intelligent, multi-agent Apps with Github and Agent Framework
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** CopilotStudio, Events GHE w/ Copilot, M365Copilot

---

# Building Intelligent Multi-Agent Apps with GitHub and Agent Framework — Lab Instruction Summary

## Exercise Summary

**Exercise 1: Explore and Test MCP Server**
- **Goal:** Validate connectivity and available tools on the hosted Model Context Protocol (MCP) server for Zava Insurance claims.
- **Actions:**
  - Launch MCP Inspector via npx command and connect to the provided MCP server URL.
  - List and review available tools (claims, inspections, contractors, purchase orders).
  - Test the `get_claims` tool to retrieve sample claims data.
- **Validation:**
  - Successful JSON response from MCP Inspector for claims data; tools are listed and accessible.

**Exercise 2: Create and Configure Declarative Agent (Claims Assistant)**
- **Goal:** Build a Microsoft 365 Declarative Agent that connects to the MCP server for claims operations.
- **Actions:**
  - Scaffold a new Declarative Agent project using Microsoft 365 Agents Toolkit in VS Code.
  - Add MCP server actions by fetching from the provided URL and select all available tools.
  - Update agent identity, instructions, and Teams app manifest for Zava branding and claims-specific logic.
- **Validation:**
  - Agent project is provisioned; agent can communicate with MCP server and respond to claims-related queries in Copilot chat.

**Exercise 3: Test and Debug Declarative Agent**
- **Goal:** Ensure the agent can process claims and interact with users via natural language.
- **Actions:**
  - Sign in to Microsoft 365 Agents Toolkit and provision the agent.
  - Test agent in Microsoft 365 Copilot with sample queries (claims lookup, inspection creation, contractor search).
  - Enable developer mode for debugging and analyze agent responses.
- **Validation:**
  - Agent responds accurately to test queries; debug info is available and correct in Copilot chat.

**Exercise 4: Create Declarative Agent with Embedded Knowledge (Procurement Assistant)**
- **Goal:** Build a procurement-focused Declarative Agent using embedded local files for contractor pricing and guidelines.
- **Actions:**
  - Scaffold a new agent project with embedded knowledge capability.
  - Download and add contractor pricing and guideline files to the `EmbeddedKnowledge` folder.
  - Update agent configuration and instructions for procurement use cases.
- **Validation:**
  - Agent can retrieve and present contractor pricing data from embedded files in response to user queries.

**Exercise 5: Build and Connect Orchestrator Agent (ZavaCare)**
- **Goal:** Create a Connected Agent that orchestrates claims and procurement agents for unified claims processing.
- **Actions:**
  - Scaffold a new Declarative Agent project for orchestration.
  - Update agent identity, instructions, and connect worker agents using their Microsoft 365 Title IDs.
  - Provision the orchestrator agent and test multi-agent workflows in Copilot chat.
- **Validation:**
  - Orchestrator agent coordinates responses from claims and procurement agents; complex queries return integrated results.

**Validation Across All Exercises:**
- Success is verified by agent responses in Copilot chat, correct data retrieval from MCP server or embedded files, and visible debug information when enabled. Provisioning and agent connectivity are confirmed via toolkit and chat interface.

