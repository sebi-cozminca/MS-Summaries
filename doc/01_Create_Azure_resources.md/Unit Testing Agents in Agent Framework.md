---
title: 'Unit Testing Agents in Agent Framework'
layout: default
nav_order: 90
parent: 'Lab summaries'
---

**ID** 208624
**Number:** LAB 182
**Name:** Unit Testing Agents in Agent Framework
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** CopilotStudio, Events GHE w/ Copilot

---

# Exercise Summary

**Exercise 1: Introduction & Environment Setup**
- **Goal:** Set up the development environment, clone the workshop repository, and configure Azure AI Foundry connectivity for agent evaluation exercises.
- **Actions:**
  - Install prerequisites: Visual Studio 2026 or VS Code with C# Dev Kit, .NET 10 SDK, Docker Desktop, Git, and Azure subscription access.
  - Clone the workshop repository using terminal, VS Code, or Visual Studio.
  - Open the solution and review the project structure.
  - Configure Azure credentials using user secrets or environment variables.
  - Start the Aspire AppHost and verify resources in the dashboard.
  - Run configuration smoke tests to validate setup.
- **Validation:**
  - Aspire AppHost dashboard is accessible with all resources healthy.
  - Configuration smoke tests pass successfully.

**Exercise 2: TaskAdherenceEvaluator**
- **Goal:** Create and run a test class using TaskAdherenceEvaluator to measure how well an AI agent completes a task.
- **Actions:**
  - Implement a test class for the Weather Assistant Agent using MSTest and BaseIntegrationTest.
  - Configure reporting and evaluators.
  - Write and run a test method to evaluate agent tool usage and response quality.
  - Update agent instructions if the test fails to improve adherence.
- **Validation:**
  - Test passes with a task adherence rating of Good or Exceptional.
  - Evaluation report confirms correct tool usage and response alignment.

**Exercise 3: Retrieval Evaluation with Built-in Evaluators**
- **Goal:** Evaluate a Knowledgebase Chat Agent using Relevance, Coherence, and Groundedness evaluators.
- **Actions:**
  - Implement a test class with multiple built-in evaluators.
  - Create a helper to provide knowledge base context from a CSV file.
  - Write data-driven tests for various question/answer scenarios.
  - Validate results for all three metrics per test case.
- **Validation:**
  - Evaluation report shows scores for all metrics.
  - Test results indicate where the agent meets or fails expectations.

**Exercise 4: Creating a Custom Evaluator**
- **Goal:** Build and integrate a custom AnswerScoringEvaluator to compare AI responses against expected answers.
- **Actions:**
  - Implement the IEvaluator interface and a custom EvaluationContext.
  - Use the LLM-as-Judge pattern to score answers.
  - Integrate the custom evaluator into the test suite alongside built-in evaluators.
  - Update test validation to include the new metric.
- **Validation:**
  - Custom evaluator scores are present in the evaluation report.
  - Test suite passes with meaningful custom metric results.

**Exercise 5: Meta-Prompt Improvement with Evaluation-Driven Development**
- **Goal:** Use an AI-powered PromptImprovementGenerator to iteratively improve agent prompts based on test failures.
- **Actions:**
  - Analyze test failures and generate improved prompts using LLM feedback.
  - Update agent instructions and rerun tests until all pass.
  - Review evaluation reports to confirm improvements.
- **Validation:**
  - All tests for the QuizGameAgent pass after prompt improvements.
  - Evaluation report shows adherence to all defined rules.

**Extension Challenges**
- **Goal:** Deepen understanding by extending evaluation scenarios and metrics.
- **Actions:**
  - Add additional evaluators (e.g., Relevance, Coherence).
  - Create edge case and parameterized tests.
  - Implement partial credit, multi-aspect, or confidence scoring in custom evaluators.
- **Validation:**
  - Extended tests and metrics provide richer evaluation insights.
  - Reports reflect nuanced agent performance across scenarios.
