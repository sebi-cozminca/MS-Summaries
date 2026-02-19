---
title: 'TechLab: Multimodal RAG with Zero Trust Part 1: Implementing Multimodal RAG'
layout: default
nav_order: 76
parent: 'Lab summaries'
---

**ID** 167996
**Number:** 1
**Name:** TechLab: Multimodal RAG with Zero Trust Part 1: Implementing Multimodal RAG
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

### Exercise Summary

**Exercise 1: Deploy an Enterprise RAG Solution**
- **Goal:** Deploy and configure a Multimodal Retrieval-Augmented Generation (RAG) solution accelerator using Azure services.
- **Actions:**
  - Sign in to the provided virtual machine and Azure portal.
  - Initialize the GPT-RAG environment using azd commands and set up Azure AI services.
  - Customize deployment by editing configuration files and adding resource tags.
  - Install and deploy the solution using azd provision and azd deploy, selecting appropriate regions and subscriptions.
  - Ingest and index multimodal data (text and images) by uploading documents, configuring environment variables, and running indexers.
  - Test the deployed chatbot for both text and image-based queries.
- **Validation:** Azure resources are provisioned, data is indexed, and the chatbot responds accurately to both text and image-based questions.

**Exercise 2: Customize the LLM Orchestration Service**
- **Goal:** Customize and redeploy the Orchestrator component to enhance system messaging and tool integration.
- **Actions:**
  - Clone the Orchestrator repository and switch to the workshop branch.
  - Edit the triage agent prompt and system message to reflect the new assistant context.
  - Add a tool for retrieving the current date in the orchestration strategy.
  - Redeploy the customized Orchestrator using azd commands and refresh the environment.
  - Test the chatbot to verify the new system message and tool functionality.
- **Validation:** The chatbot displays the custom system message and correctly answers queries requiring the current date, confirming successful customization and redeployment.
