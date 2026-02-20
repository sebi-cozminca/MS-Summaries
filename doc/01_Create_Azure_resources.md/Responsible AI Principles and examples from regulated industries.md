---
title: 'Responsible AI Principles and examples from regulated industries'
layout: default
nav_order: 46
parent: 'Lab summaries'
---

**ID** 208626  
**Number:** LAB 184  
**Name:** Responsible AI Principles and examples from regulated industries  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Azure AI Foundry Hands-on Lab**
- **Goal:** Build, evaluate, and monitor a responsible AI agent using Azure AI Foundry and implement guardrails for regulated industry scenarios.
- **Actions:**
  - Sign in to Azure Portal and assign the Azure AI User role to managed identities for Foundry resources.
  - Access Azure AI Foundry workspace, verify model deployments, and create a new agent using GPT-4o with healthcare insurance data.
  - Configure Application Insights monitoring and enable continuous evaluation with selected evaluators and judge model.
  - Test the agent in the Playground and review traces and evaluation metrics.
  - Create and assign Responsible AI guardrails (e.g., PII protection, content safety) to the agent, and test guardrail enforcement with sample prompts.
  - Monitor evaluation and operational metrics to ensure responsible agent behavior.
- **Validation:**
  - Agent is created, monitored, and evaluated in Foundry; guardrails block or warn on unsafe prompts; evaluation metrics and traces are visible in the portal.

**Exercise 2: Data Query Agent - RAI Compliant**
- **Goal:** Set up and run a data query agent in a local VS Code environment, ensuring Responsible AI compliance.
- **Actions:**
  - Open the Data Query Agent project in VS Code and configure environment variables using Azure Foundry endpoint and API key.
  - Run the Jupyter notebook (`data_query_system.ipynb`) with the correct Python virtual environment, executing cells and testing agent queries.
  - Troubleshoot environment issues (missing packages, virtual environment setup) as needed.
- **Validation:**
  - Notebook runs successfully, agent responds to queries, and environment issues are resolved using provided troubleshooting steps.

**Optional: Pro-code Agent Integration**
- **Goal:** Integrate and test a code-first Foundry agent using Python scripts and Azure resources.
- **Actions:**
  - Set up the Foundry Agent codebase, configure `.env` with project endpoint and Application Insights connection string.
  - Activate Python virtual environment, log in to Azure, and run scripts to create and interact with the agent.
  - Verify agent creation in Foundry portal, enable evaluation, and test chat conversation via code.
- **Validation:**
  - Agent is created and visible in Foundry, chat interactions work via code, and evaluation metrics are available in the portal.
