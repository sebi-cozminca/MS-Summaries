---
title: 'Zero to Hero: Hands-on with GitHub Copilot'
layout: default
nav_order: 94
parent: 'Lab summaries'
---

**ID** 208635  
**Number:** LAB 333  
**Name:** Zero to Hero: Hands-on with GitHub Copilot  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Copilot Basics**
- **Goal:** Learn foundational GitHub Copilot features and improve test coverage in a TypeScript/Express project.
- **Actions:**
  - Log in to GitHub and create a new repository from a template.
  - Clone the repository and open it in VS Code.
  - Install dependencies using `make install`.
  - Enable and verify GitHub Copilot in VS Code.
  - Use Copilot code completions to add new tests to `branch.test.ts`.
  - Use Copilot Chat (Edit mode, Auto model) to generate a new test file for `product.ts` by referencing existing test patterns and API schemas.
  - Review, refine, and run the generated tests with `make test`.
- **Validation:**
  - New and existing tests run successfully and follow project patterns.
  - Copilot is enabled and providing suggestions.

**Exercise 2: Agent Mode**
- **Goal:** Implement a new shopping cart feature using Copilot's Plan and Agent modes with visual context.
- **Actions:**
  - Start the application and review the current Products page.
  - Use Copilot Chat in Plan mode, attach a design image, and prompt for a Cart feature plan.
  - Review and refine the implementation plan.
  - Switch to Agent mode and let Copilot autonomously implement the cart feature across multiple files.
  - Review, accept, or modify Copilot's code changes.
  - Test the new cart functionality in the running application.
- **Validation:**
  - Cart icon and page are present and functional.
  - Cart actions (add, remove, view items) work as expected.

**Exercise 3: GitHub Platform and Agentic AI**
- **Goal:** Leverage GitHub Copilot's platform features for asynchronous development, code review, and security.
- **Actions:**
  - Create a GitHub Issue for a new feature and assign it to Copilot Coding Agent.
  - Monitor Copilot's progress as it implements the feature and opens a draft PR.
  - Review Copilot's PR, code changes, and screenshots.
  - Use Copilot Code Review for AI-powered feedback and suggestions.
  - Learn about Copilot Autofix for security vulnerabilities and orchestrate multiple agent tasks in parallel.
- **Validation:**
  - Feature is implemented and PR is ready for review.
  - Copilot Code Review provides actionable feedback.
  - Security vulnerabilities are identified and fixed automatically.

**What's Next: Advanced Copilot Features**
- **Goal:** Explore advanced Copilot capabilities and resources for continued learning.
- **Actions:**
  - Review and experiment with custom instructions, custom agents, MCP servers, Copilot CLI, Copilot Memory, and Copilot Spaces.
  - Access documentation, community resources, and best practices for prompt engineering.
- **Validation:**
  - Advanced features are understood and available for future use.
  - Resources and documentation are accessible for ongoing mastery.
