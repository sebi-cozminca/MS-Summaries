---
title: 'TechLab: Transform your processes with Microsoft Copilot Studio'
layout: default
nav_order: 81
parent: 'Lab summaries'
---

**ID** 186383
**Number:** LAB216
**Name:** TechLab: Transform your processes with Microsoft Copilot Studio
**CloudSubscriptionPoolName:** TechMaster MSLEARN - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** Copilot Studio Tenants (2025 Batch 1)
**Additional licenses:** NA

---

# TechLab Transform your processes with Microsoft Copilot Studio — Exercise Summary

## Exercise Summary

**Exercise 1: Build Your First Agent**
- **Goal:** Create a generative AI-powered agent in Microsoft Copilot Studio and configure it with external knowledge sources.
- **Actions:**
  - Sign in to Copilot Studio and create a new agent.
  - Add a public website as a knowledge source.
  - Test the agent with a sample query.
- **Validation:**
  - Agent responds accurately to test queries using generative answers.

**Exercise 2: Publish the Agent**
- **Goal:** Publish the agent and make it available in Microsoft Teams.
- **Actions:**
  - Publish the agent from Copilot Studio.
  - Add the agent to Teams via the Channels tab.
  - Test the agent in Teams with a sample question.
- **Validation:**
  - Agent is accessible and functional in Microsoft Teams; responses are validated in the Teams interface.

**Exercise 3: Extend the Agent with Custom Connectors**
- **Goal:** Build and test a custom API connector to extend agent capabilities.
- **Actions:**
  - Open and build the ContosoApiApp solution in Visual Studio.
  - Run and test the API locally, verifying GET method functionality.
- **Validation:**
  - API methods return expected results in the local test interface.

**Exercise 4: Add a New Method to the Connector**
- **Goal:** Add and validate a method for updating order delivery addresses in the API.
- **Actions:**
  - Implement the UpdateDeliveryAddress method in OrderController.cs.
  - Run and test the new POST method locally.
- **Validation:**
  - POST method updates and returns order details as expected in the test interface.

**Exercise 5: Add the Connector to Microsoft Copilot Studio**
- **Goal:** Register and configure the custom connector in Copilot Studio for agent use.
- **Actions:**
  - Switch API run mode to HTTPS.
  - Add the connector to Microsoft Power Platform via Visual Studio.
  - Create a dev tunnel and complete connector setup.
- **Validation:**
  - Connector is available in Copilot Studio for use in agent actions.

**Exercise 6: Add the Contoso Plugin to the Agent**
- **Goal:** Integrate and test the custom connector's actions within the agent.
- **Actions:**
  - Enable generative AI orchestration in Copilot Studio settings.
  - Add both Get Order Details and Update Delivery Address actions to the agent.
  - Test the agent's new capabilities using the conversation map and activity map.
- **Validation:**
  - Agent successfully calls connector actions and returns correct results for order queries and address updates.

**Lab Completion**
- **Validation:**
  - Submit the lab in the Skillable platform and confirm completion status in Viva and Learning Path the following week.
