---
title: 'Project Plaid: Secure, extensible framework for AI-first delivery'
layout: default
nav_order: 45
parent: 'Lab summaries'
---

**ID** 208621  
**Number:** LAB 112  
**Name:** Project Plaid: Secure, extensible framework for AI-first delivery  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise Blank Admin Only 15S (Stakeholder: Kim Frank)  
**Additional licenses:** CopilotStudio, Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Log into Lab Environment and GitHub**
- **Goal:** Access the lab virtual machine and authenticate with GitHub for VS Code extension development.
- **Actions:**
  - Log into the provided Windows VM using lab credentials.
  - Authenticate to GitHub via browser and connect VS Code to GitHub using Azure credentials.
- **Validation:**
  - Successful access to VS Code, GitHub Copilot, and the extension marketplace.

**Exercise 2: Prompt Picker Extension - Setup and Build**
- **Goal:** Prepare the Prompt Picker extension for development and testing in VS Code.
- **Actions:**
  - Open the Prompt Picker Extension folder in VS Code.
  - Install dependencies with `npm install` and compile with `npm run compile`.
- **Validation:**
  - Extension compiles without errors and is ready for development.

**Exercise 3: Test Extension Changes**
- **Goal:** Test extension modifications using both development host and VSIX packaging methods.
- **Actions:**
  - Use Extension Development Host (Fn+F5) for quick testing.
  - Package and install the extension as a VSIX for persistent testing.
- **Validation:**
  - Extension loads in VS Code and changes are visible in the test environment.

**Exercise 4: Lab Exercises (Choose 2-3)**
- **Goal:** Practice making and testing changes to the Prompt Picker extension.
- **Actions:**
  - Add a startup notification message in `src/extension.ts`.
  - Add a new built-in prompt in `src/data/builtinPrompts.ts`.
  - Change the chat participant icon in `src/chat/prompt-picker-chat-participant.ts`.
  - Add a welcome message to chat in `src/chat/prompt-picker-chat-participant.ts`.
  - Add a new chat command (advanced) by editing `package.json` and `src/chat/prompt-picker-chat-participant.ts`.
- **Validation:**
  - Each change is compiled, tested, and verified in the Extension Development Host.

**Exercise 5: Publish to Private Marketplace**
- **Goal:** Publish the Prompt Picker extension to the Project Plaid private marketplace.
- **Actions:**
  - Use Plaid CLI or the `plaidcli-assistant` agent to publish the extension.
  - Verify the extension appears in the private marketplace and is discoverable in VS Code.
- **Validation:**
  - Extension is listed in the private marketplace and available for installation by others.

**Exercise 6: AI First MCP Tool Gateway Extension**
- **Goal:** Use the AI First MCP Tool Gateway extension to access MCP tools in Copilot Agent Mode.
- **Actions:**
  - Verify the AIFirstMCPServer is installed and running in VS Code.
  - Use Copilot Chat in Agent Mode to invoke MCP tools (e.g., weather tool).
- **Validation:**
  - MCP tools are accessible and respond to queries in Copilot Agent Mode.

**Optional Exercise: Create and Publish a New Chat Participant with Plaid CLI**
- **Goal:** Use Plaid CLI to create, install, and publish a new chat participant extension.
- **Actions:**
  - List, create, install, and publish a chat participant using Plaid CLI commands or the plaidcli-assistant agent.
  - Verify the new participant is available in VS Code and the private marketplace.
- **Validation:**
  - New chat participant is functional and published to the marketplace.
