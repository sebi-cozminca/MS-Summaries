---
title: 'Using the AI Migrate Copilot Agents'
layout: default
nav_order: 91
parent: 'Lab summaries'
---

**ID** 208643
**Number:** LAB 482
**Name:** Using the AI Migrate Copilot Agents
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** CopilotStudio, E3, M365Copilot

---

# Exercise Summary

**Exercise 0: Prerequisites and SharePoint Setup**
- **Goal:** Prepare the environment and SharePoint site for agent operation.
- **Actions:**
  - Sign in to Microsoft 365 and create a SharePoint Team site.
  - Set up required document folders (Intake-Documents, Architecture-Documents).
- **Validation:**
  - SharePoint site and folders are accessible and ready for use.

**Exercise 1: Solution Import**
- **Goal:** Import Intake Agent and Design Agent solutions into Copilot Studio.
- **Actions:**
  - Access Copilot Studio and select/create a development environment.
  - Import IntakeAgent and DesignAgent solution packages.
  - Update agent tool settings and configure agent models.
- **Validation:**
  - Both agents appear in Copilot Studio and are configured as specified.

**Exercise 2: Connection Configuration**
- **Goal:** Establish and verify all required agent connections.
- **Actions:**
  - Connect Office 365 Outlook for Intake Agent.
  - Connect Microsoft Learn Docs MCP and Save Design Document for Design Agent.
  - Configure and publish Power Automate flows for document processing.
- **Validation:**
  - All connections show "Connected" status and flows are published.

**Exercise 3: Knowledge Base Setup**
- **Goal:** Upload and configure knowledge base files for both agents.
- **Actions:**
  - Add and verify knowledge files in the Knowledge tab for each agent.
- **Validation:**
  - Knowledge status displays as "Ready" for both agents.

**Exercise 4: Testing the Agents**
- **Goal:** Validate agent operation in interactive mode.
- **Actions:**
  - Test Intake Agent by uploading a sample document and responding to agent prompts.
  - Test Design Agent by generating a design document from intake data.
- **Validation:**
  - Agents generate expected summaries and architecture documents in chat.

**Exercise 5: Autonomous Agent Mode**
- **Goal:** Enable and test autonomous document processing.
- **Actions:**
  - Configure triggers for the Design Agent to process new SharePoint documents automatically.
  - Upload intake documents to SharePoint and monitor flow execution.
- **Validation:**
  - Design documents are automatically generated and saved in the correct SharePoint folder.

**Exercise 6: Topic Walkthrough**
- **Goal:** Understand and customize the main topic flow for architecture generation.
- **Actions:**
  - Review and modify topic nodes, prompts, and Power Automate actions in Copilot Studio.
- **Validation:**
  - Topic flow produces the expected architecture document structure and can be tailored as needed.

**Exercise 7: Add Cost Estimation Topic**
- **Goal:** Extend the Design Agent to generate Azure cost estimation sections.
- **Actions:**
  - Enable web search and add a Generative Answers node for cost estimation.
  - Configure prompts, variables, and output formatting for cost tables and summaries.
- **Validation:**
  - Generated documents include a cost estimation section with tables and recommendations.

**Exercise 8: Understanding the Output**
- **Goal:** Interpret the structure and content of generated architecture documents.
- **Actions:**
  - Review document sections: introduction, data flows, five architecture views, rationales, and Azure resource tables.
- **Validation:**
  - All required sections are present and formatted for deployment and stakeholder review.

**Exercise 9: Publishing to Channels**
- **Goal:** Make the agents available across organizational channels.
- **Actions:**
  - Publish the Design Agent in Copilot Studio.
  - Enable publishing to Teams, SharePoint, Power Apps, and Microsoft 365 Copilot.
- **Validation:**
  - Agents are accessible in selected channels and available to target audiences.

**Appendix: Troubleshooting and Analytics**
- **Goal:** Resolve common issues and monitor agent performance.
- **Actions:**
  - Use provided troubleshooting steps for connection, extraction, and flow errors.
  - Monitor analytics for run success rates and performance metrics.
- **Validation:**
  - Issues are resolved promptly and agent performance meets targets.
