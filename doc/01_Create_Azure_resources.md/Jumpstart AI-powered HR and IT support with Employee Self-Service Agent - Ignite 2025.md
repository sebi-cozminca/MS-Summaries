---
title: 'Jumpstart AI-powered HR and IT support with Employee Self-Service Agent - Ignite 2025'
layout: default
nav_order: 32
parent: 'Lab summaries'
---

**ID** 205506  
**Number:** LAB562  
**Name:** Jumpstart AI-powered HR and IT support with Employee Self-Service Agent - Ignite 2025  
**CloudSubscriptionPoolName:** LAB562 Recycling Pool  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** CopilotStudio, Ignite25_Lab562  

---

## Exercise Summary

**Exercise 1: Environment Setup and Copilot Studio Access**
- **Goal:** Prepare the lab environment and access Copilot Studio for agent configuration.
- **Actions:**
  - Log into the provided virtual machine and access Copilot Studio via Microsoft Edge.
  - Complete initial setup, region selection, and cancel default agent creation.
  - Verify developer environment readiness.
- **Validation:**
  - Copilot Studio displays "Environment - [your user ID]" in the upper-right corner.

**Exercise 2: Install Employee Self-Service Agents**
- **Goal:** Deploy HR and IT Employee Self-Service starter agents in Copilot Studio.
- **Actions:**
  - Navigate to Agents and install both Employee Self-Service HR and IT agents.
  - Confirm installation and close dialogs.
- **Validation:**
  - Both agents appear in the Agents list and are accessible.

**Exercise 3: SharePoint Site Familiarization**
- **Goal:** Review sample content provided for the lab in SharePoint.
- **Actions:**
  - Open the specified SharePoint site and review sample documents in the Documents section.
- **Validation:**
  - Access to and review of sample SharePoint content is confirmed.

**Exercise 4: Test and Configure the HR Agent**
- **Goal:** Interact with and configure the Employee Self-Service HR agent.
- **Actions:**
  - Open the HR agent and use sample prompts in the Test pane.
  - Add SharePoint as a knowledge source to the agent.
  - Review agent instructions and user context handling.
- **Validation:**
  - Agent responds accurately to sample prompts and reflects knowledge source integration.

**Exercise 5: Set and Change User Context**
- **Goal:** Demonstrate user context configuration and its effect on agent responses.
- **Actions:**
  - Set user context variables (e.g., Level, Country Code) in the agent's topic.
  - Test agent responses with different context values.
- **Validation:**
  - Agent responses change appropriately based on user context settings.

**Exercise 6: Configure Crafted and Sensitive Responses**
- **Goal:** Implement crafted and sensitive topic handling in the agent.
- **Actions:**
  - Enable and edit the crafted response topic for compensation-related queries.
  - Review and test the sensitive topics catch-all configuration.
- **Validation:**
  - Official answers are provided for sensitive prompts; crafted responses trigger as specified.

**Exercise 7: Set Message-Level Disclaimers**
- **Goal:** Add and customize disclaimers for agent responses.
- **Actions:**
  - Update the disclaimer variable in the response preparation topic.
- **Validation:**
  - Customized disclaimer appears in agent responses as configured.

**Exercise 8: Install Accelerator Packs and Integrations**
- **Goal:** Extend agent functionality with ServiceNow HR accelerator pack.
- **Actions:**
  - Install ServiceNow HR accelerator pack and configure authentication.
  - Review new topics and workflows added by the pack.
- **Validation:**
  - ServiceNow HRSD topics are present and functional in the agent.

**Exercise 9: Set Up Agent Handoff**
- **Goal:** Enable agent handoff to M365 Copilot for specific scenarios.
- **Actions:**
  - Retrieve and configure the handoff agent ID from M365 Copilot.
  - Enable and customize the agent handoff topic and test the handoff experience.
- **Validation:**
  - Handoff to the Researcher Agent works as expected for relevant prompts.

**Exercise 10: Configure Starter Prompts and Publish Agent**
- **Goal:** Finalize agent configuration and publish to Teams and M365 Copilot.
- **Actions:**
  - Update starter prompts for the Employee Self-Service agent.
  - Publish the agent and configure channel details, including name, icon, and disclaimers.
- **Validation:**
  - Agent is published and available in Teams and M365 Copilot with correct configuration.