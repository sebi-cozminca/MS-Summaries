---
title: 'Autonomous Identity Hardening with Microsoft Entra Security Agents'
layout: default
nav_order: 4
parent: 'Lab summaries'
---

**ID** 208637
**Number:** LAB 408
**Name:** Autonomous Identity Hardening with Microsoft Entra Security Agents
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** CopilotStudio, E5

---

### Exercise Summary

**Lab Overview:**
- **Goal:** Build a Tier 2 SOC Analyst Agent in Microsoft Copilot Studio to automate identity threat detection and policy auditing using generative AI.
- **Actions:**
  - Prepare three data files: a high-risk user watch list (CSV), sign-in logs (JSON), and complex Conditional Access policies (JSON).
  - Understand the agent's objectives: cross-reference logs, classify attacks with MITRE ATLAS, and audit Conditional Access policies for compliance.
- **Validation:**
  - Data files are created and ready for upload; objectives and prerequisites are clear.

**Phase 1: Agent Setup & Knowledge Injection**
- **Goal:** Create and configure the agent with required knowledge sources and persona.
- **Actions:**
  - Create a blank agent in Copilot Studio and wait for provisioning.
  - Add the watch list CSV and MITRE ATLAS website as knowledge sources.
  - Set agent name, description, and detailed instructions for analysis, tone, and response format.
- **Validation:**
  - Agent is provisioned, knowledge sources are listed, and persona/instructions are saved.

**Phase 2: Building the Analysis Capabilities**
- **Goal:** Implement agent skills for log analysis and Conditional Access policy auditing.
- **Actions:**
  - Create a "Sign-in Log Analysis" topic: prompt for JSON logs, save input, and use generative AI for analysis.
  - Create a "CA Policy Audit" topic: prompt for JSON policies, save input, and use generative AI for compliance checks.
- **Validation:**
  - Topics are created, logic flows are configured, and agent is ready to process user-provided data.

**Phase 3: Testing (The Walkthrough)**
- **Goal:** Validate agent's ability to detect threats and compliance gaps using test scenarios.
- **Actions:**
  - Test log analysis: submit sign-in logs and verify watch list detection, MITRE classification, and response format.
  - Test policy audit: submit Conditional Access policies and verify detection of exclusions, report-only gaps, and compliance conclusions.
- **Validation:**
  - Agent produces structured, actionable alerts and compliance findings as specified in the instructions.

**Lab Complete:**
- **Goal:** Confirm the agent can autonomously cross-reference logs, classify threats, and audit policies.
- **Actions:**
  - Review agent outputs for both scenarios and ensure all success criteria are met.
- **Validation:**
  - Agent meets all functional requirements and demonstrates autonomous identity hardening capabilities.
