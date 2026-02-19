---
title: 'TechLab: Declarative Agents: Build Agents for Microsoft 365 Copilot'
layout: default
nav_order: 62
parent: 'Lab summaries'
---

**ID** 186385
**Number:** LAB910
**Name:** TechLab: Declarative Agents: Build Agents for Microsoft 365 Copilot
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)
**AllowSave:** False
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise Blank Admin Only 15S (Stakeholder: Kim Frank)
**Additional licenses:** TreyLegalDocsReaders, TrialFabricUsers

---

### Exercise Summary

**Exercise 1: Run the starting solution**
- **Goal:** Launch and validate the initial declarative agent and API plugin in Microsoft 365 Copilot using Visual Studio Code and Teams Toolkit.
- **Actions:**
  - Open the starter project in VS Code and sign in to Microsoft 365.
  - Set up local environment files and start a debug session.
  - Test API endpoints using the provided HTTP test file.
  - Run the solution in Copilot, approve API plugin consent, and interact with the agent using sample prompts.
- **Validation:**
  - API responses are returned as expected; Copilot agent responds to prompts and displays consultant/project data.

**Exercise 2: Add instructions and SharePoint files**
- **Goal:** Enhance the agent with additional instructions and integrate SharePoint document knowledge.
- **Actions:**
  - Update agent instructions in the JSON config to include company motto.
  - Add SharePoint site reference to agent capabilities for document access.
  - Provision a new version of the agent and update its name.
  - Test the updated agent in Copilot with prompts that require SharePoint knowledge.
- **Validation:**
  - Agent responses include SharePoint document content and the Trey motto; new agent version is selectable in Copilot.

**Exercise 3: Add project API**
- **Goal:** Extend the API plugin and agent to support project-related queries and actions.
- **Actions:**
  - Implement a new Azure Function endpoint for /projects.
  - Add /projects endpoints to the HTTP test file for validation.
  - Update the OpenAPI definition with new /projects GET and POST endpoints.
  - Add project-related functions and adaptive card templates to the API plugin file.
  - Update the agent config and provision a new version.
  - Test API endpoints and agent project queries in Copilot.
- **Validation:**
  - API returns project data; Copilot agent can answer project-related prompts and perform project assignments using the new endpoints.
