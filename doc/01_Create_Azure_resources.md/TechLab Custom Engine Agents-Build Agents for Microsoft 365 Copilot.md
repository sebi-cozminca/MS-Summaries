---
title: 'TechLab: Custom Engine Agents-Build Agents for Microsoft 365 Copilot'
layout: default
nav_order: 61
parent: 'Lab summaries'
---

**ID** 186550  
**Number:** LAB911  
**Name:** TechLab: Custom Engine Agents-Build Agents for Microsoft 365 Copilot  
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** TC LAB911 Cred Pool  
**Additional licenses:** TrialFabricUsers  

---

## Exercise Summary

**Exercise 1: Create a custom engine agent**
- **Goal:** Build and provision a custom Teams AI agent using Visual Studio, Teams Toolkit, and Azure resources.
- **Actions:**
  - Open and examine the starter project in Visual Studio 2022.
  - Set up a Dev Tunnel for secure local development.
  - Review and execute Teams Toolkit provisioning tasks to register and provision Teams and Azure resources.
  - Deploy Azure OpenAI resources and configure environment variables for agent integration.
  - Update Azure bot Bicep configuration and complete provisioning.
- **Validation:**
  - Azure Bot and Azure OpenAI resources are provisioned; agent project is ready for debugging and deployment.

**Exercise 2: Running the Custom Engine Agent**
- **Goal:** Run and test the custom engine agent in Microsoft Teams.
- **Actions:**
  - Configure solution for multi-project startup and start a debug session.
  - Install and open the agent in Microsoft Teams.
  - Interact with the agent and observe AI-generated responses.
  - Review conversation tracking in Visual Studio debug output.
- **Validation:**
  - Agent responds to messages in Teams; debug output shows conversation history.

**Exercise 3: Prompt templates**
- **Goal:** Customize agent behavior by updating prompt templates.
- **Actions:**
  - Edit the default prompt template to change agent persona and response style.
  - Test the updated prompt by running the agent and sending sample messages.
- **Validation:**
  - Agent responses reflect new persona and behavior as defined in the prompt template.

**Exercise 4: Suggested prompts**
- **Goal:** Enhance user experience by adding suggested prompts to the agent UI.
- **Actions:**
  - Update Teams app manifest to define suggested prompts.
  - Run Teams Toolkit dependency preparation and debug the agent.
  - Verify suggested prompts appear in Teams and function as intended.
- **Validation:**
  - Suggested prompts are visible and usable in the Teams agent interface.

**Exercise 5: Message handlers**
- **Goal:** Implement custom message handlers for specific user commands.
- **Actions:**
  - Create a message handler to clear conversation history on receiving a "/new" command.
  - Register the handler in the agent setup code.
  - Debug and test the handler by sending the command in Teams.
- **Validation:**
  - Agent responds with a fixed message and clears conversation history when "/new" is sent.
