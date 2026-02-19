---
title: 'Automate your enterprise workflows with MCP Tools'
layout: default
nav_order: 3
parent: 'Lab summaries'
---

**ID** 205917
**Number:** Lab572
**Name:** Automate your enterprise workflows with MCP Tools
**CloudSubscriptionPoolName:** M365 Labs CSR
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** M365Copilot, CopilotStudio, E3

---

### Exercise Summary

**Lab Setup:**
- **Goal:** Prepare the environment and required Microsoft services for agent and MCP server configuration.
- **Actions:**
  - Log into the virtual machine and set up Copilot Studio in an InPrivate browser session.
  - Start Copilot Studio initialization and cancel agent creation to allow background setup.
  - Set up Outlook with provided credentials for later email/calendar integration.
- **Validation:**
  - Copilot Studio and Outlook are accessible and ready for use.

**Scenario 1: Create and Configure an Agent**
- **Goal:** Build and configure a Microsoft Copilot Studio agent for targeted workflow automation.
- **Actions:**
  - Sign in to Copilot Studio and select the correct environment.
  - Create a new agent (via button or chat panel, depending on UI version).
  - Configure agent settings: disable web search, set content moderation to low, and restrict knowledge to server-based responses only.
  - Save and close agent configuration.
- **Validation:**
  - Agent is created, settings are saved, and agent is ready for MCP server integration.

**Scenario 2: Add MCP Servers to an Agent**
- **Goal:** Integrate and test MCP servers for email, calendar, and file management automation within the agent.
- **Actions:**
  - Add the Email Management MCP Server, authenticate with Outlook, and test sending an email via the agent.
  - Add Meeting Management and SharePoint/OneDrive MCP servers, configure connections, and test file listing and sharing.
  - Combine servers in multi-step instructions (e.g., send resume links, schedule meetings, send reminders).
  - Add Microsoft 365 Copilot (Search) MCP for document content summarization and advanced workflow automation.
  - Test complex, multi-server scenarios (summarize documents, send emails, create meetings with contextual data).
  - Publish the agent and select channels for deployment.
- **Validation:**
  - Agent successfully performs automated tasks across email, calendar, and file management; published agent is available for use in selected channels.
