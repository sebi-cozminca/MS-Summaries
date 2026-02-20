---
title: 'Validating and Testing the Quality of Copilot Agents with Evals'
layout: default
nav_order: 92
parent: 'Lab summaries'
---

**ID** 208644  
**Number:** LAB 484  
**Name:** Validating and Testing the Quality of Copilot Agents with Evals  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** M365Copilot, CopilotStudio, E3, Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Copilot Studio Evaluation**
- **Goal:** Configure and run Copilot Studio Evaluation on an HR Self-Service agent to assess response quality and identify improvement areas.
- **Actions:**
  - Create a new Power Platform environment and provision Copilot Studio.
  - Import the HR Self-Service agent solution and test dataset.
  - Run an automated evaluation using Copilot Studio's built-in test methods (ExactMatch, PartialMatch, TextSimilarity, CompareMeaning, GeneralQuality).
  - Review evaluation results, including scores and conversation transcripts.
  - Optionally, create new evaluations with AI-assisted test set generation.
- **Validation:**
  - Evaluation completes with detailed metrics and conversation analysis available for each test case.

**Exercise 2: Evaluating a Custom HR Self-Service Agent with AutoEval**
- **Goal:** Use AutoEval to measure and improve the quality of a Copilot Studio HR Self-Service agent.
- **Actions:**
  - Create a declarative HR agent in Copilot Chat with SharePoint and web knowledge sources.
  - Set up and launch AutoEval, create a workspace, and provision Azure resources.
  - Import and edit the test dataset, then run the evaluation.
  - Analyze results, including detailed chat simulations and difference analysis.
  - Update agent settings to restrict knowledge sources and rerun the evaluation for improved results.
- **Validation:**
  - AutoEval produces quality metrics (Answer Accuracy, Relevancy, Context Recall, Domain Rubrics) and detailed analysis, showing improvement after agent updates.

**Exercise 3: Evaluating Agents with Microsoft Foundry SDK (Preview)**
- **Goal:** Evaluate an AI agent using the Microsoft Foundry SDK and compare results before and after enhancements.
- **Actions:**
  - Set up the environment with Python, Azure CLI, and VS Code.
  - Launch Jupyter Notebook and open Eval_Agent.ipynb.
  - Follow notebook steps to create, evaluate, and enhance a Foundry agent.
  - Add file search and policy documents to the agent, then re-evaluate.
- **Validation:**
  - Notebook outputs confirm successful agent creation, evaluation, and measurable improvement after enhancements.
