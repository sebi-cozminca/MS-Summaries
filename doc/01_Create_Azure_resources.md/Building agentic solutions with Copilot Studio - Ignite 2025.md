---
title: 'Building agentic solutions with Copilot Studio - Ignite 2025'
layout: default
nav_order: 11
parent: 'Lab summaries'
---

**ID** 205047  
**Number:** LAB570  
**Name:** Building agentic solutions with Copilot Studio - Ignite 2025  
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** E5, Microsoft 365 Copilot  

---

## Exercise Summary

**Exercise 0: Configure the Environment**
- **Goal:** Set up the Copilot Studio and supporting environment for agent development.
- **Actions:**
  - Sign in to the provided virtual machine and Microsoft Edge.
  - Access Power Platform admin portal and create a new environment for Zava.
  - Wait for environment readiness and record the Environment ID.
- **Validation:**
  - Environment is visible and in 'Ready' state; Environment ID is recorded.

**Exercise 1: Build Your Agent**
- **Goal:** Create a Copilot Studio agent with custom knowledge and instructions.
- **Actions:**
  - Access Copilot Studio and create a new agent named Zava Order Support.
  - Upload company knowledge documents (FAQ, returns, shipping, warranty policies).
  - Add detailed instructions to guide agent behavior and disable general knowledge.
  - Test the agent to ensure it answers using only provided knowledge sources.
- **Validation:**
  - Agent answers questions with citations from uploaded documents; general knowledge is not used.

**Exercise 2: Connect to an MCP Server**
- **Goal:** Integrate the agent with a live MCP server for inventory and store management.
- **Actions:**
  - Explore and run the Zava Inventory MCP server in VS Code.
  - Expose the local server via a dev tunnel for public access.
  - Register the MCP server as a tool in Copilot Studio and configure API key authentication.
  - Test agent actions such as listing stores, querying inventory, and adding new stores.
- **Validation:**
  - Agent successfully triggers MCP tools and updates are reflected in the backend data files.

**Exercise 3: Add a Prompt for Warranty Claim Processing**
- **Goal:** Enable the agent to process warranty claims using an AI prompt for information extraction.
- **Actions:**
  - Add a new Prompt tool for warranty claim processing.
  - Configure the prompt to extract structured claim details from unstructured text.
  - Set output to JSON and test with sample data.
  - Update agent instructions to call the prompt and reference warranty policy knowledge.
- **Validation:**
  - Agent extracts and returns structured claim information and policy details in response to warranty claim requests.

**Exercise 4: Add an Agent Flow for Approving Warranty Claims**
- **Goal:** Automate warranty claim approval using an agent flow based on extracted claim data and policy rules.
- **Actions:**
  - Create an Agent Flow with inputs for issue category, purchase date, and coverage window.
  - Implement logic to auto-approve or escalate claims based on conditions.
  - Connect the flow to the agent and update instructions to use it after claim extraction.
- **Validation:**
  - Agent calls the flow, returns approval outcome and message, and informs the user of the process.

**Exercise 5: Test Your Agent**
- **Goal:** Validate the end-to-end agent workflow for order management and warranty claims.
- **Actions:**
  - Test the agent with various scenarios in the Test Panel.
  - Confirm correct tool and flow invocations and appropriate responses for different claim conditions.
- **Validation:**
  - Agent demonstrates knowledge retrieval, MCP integration, prompt-based extraction, and flow-based approval in test cases.