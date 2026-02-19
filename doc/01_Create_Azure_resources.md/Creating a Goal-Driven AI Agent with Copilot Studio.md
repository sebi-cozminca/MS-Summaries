---
title: 'Creating a Goal-Driven AI Agent with Copilot Studio'
layout: default
nav_order: 20
parent: 'Lab summaries'
---

**ID** 205042
**Number:** LAB 631
**Name:** Creating a Goal-Driven AI Agent with Copilot Studio
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot, M365Copilot, CopilotStudio, E3

---

# Creating a Goal-Driven AI Agent with Copilot Studio — Lab Instruction Summary

## Exercise Summary

**Exercise 1: Understanding Topic Architecture**
- **Goal:** Learn the structure and design of intelligent topic routing in Copilot Studio using AI Builder.
- **Actions:**
  - Study topic components (trigger phrases, flows, variables, actions).
  - Plan an AI Builder model for intent analysis and topic redirection.
- **Validation:**
  - Clear understanding of topic modularity and AI-driven routing logic.

**Exercise 2: Creating a New Agent in Copilot Studio**
- **Goal:** Set up a new Copilot Studio agent for extensibility guidance.
- **Actions:**
  - Access Copilot Studio and create a new agent.
  - Configure agent model, details, instructions, conversation starters, and settings (orchestration, knowledge, etc.).
- **Validation:**
  - Agent is provisioned, configured, and ready for topic and AI enhancements.

**Exercise 3: Creating the AI Builder Model**
- **Goal:** Implement AI Builder for user intent analysis and dynamic topic routing.
- **Actions:**
  - Create the "Intent Analysis" topic and child topics for no-code/low-code and pro-code paths.
  - Add and configure an AI Builder prompt for intent classification.
  - Bind input/output variables and build conversation flow with conditional redirection.
- **Validation:**
  - User input is analyzed and routed to the correct topic based on intent; fallback for unclear input is handled.

**Exercise 4: Testing the Conversational Flow**
- **Goal:** Validate the agent’s ability to route conversations based on user intent.
- **Actions:**
  - Publish and test the agent using sample prompts for both no-code and pro-code scenarios.
- **Validation:**
  - Agent routes to the correct topic and displays the expected response for each test case.

**Part 2: Building Custom Topics with Generative Answers**

**Exercise 1: Setting Up SharePoint Document Library as Knowledge Source**
- **Goal:** Integrate SharePoint document libraries as knowledge sources for generative answers.
- **Actions:**
  - Browse SharePoint libraries and add them as knowledge sources in Copilot Studio.
  - Configure names and descriptions for each knowledge source.
- **Validation:**
  - Knowledge sources are added and show "Ready" status in the agent.

**Exercise 2: Adding Generative Answers to Existing Topics**
- **Goal:** Enhance topics with Generative Answers actions for targeted knowledge-based responses.
- **Actions:**
  - Edit No-Code/Low-Code and Pro-Code topics to add Generative Answers actions.
  - Configure each action to use the appropriate SharePoint knowledge source and store responses in variables.
- **Validation:**
  - Generative Answers actions return targeted responses from the correct knowledge base.

**Exercise 3: Customizing Output with PowerFx and Adaptive Cards (Bonus)**
- **Goal:** Format and present generative responses using PowerFx and Adaptive Cards.
- **Actions:**
  - Disable default message in Generative Answers and add an Adaptive Card to the topic.
  - Use PowerFx formulas to bind dynamic content to the card.
  - Test the enhanced topic for correct rendering and content.
- **Validation:**
  - Adaptive Card displays structured, formatted responses with dynamic content and references.
