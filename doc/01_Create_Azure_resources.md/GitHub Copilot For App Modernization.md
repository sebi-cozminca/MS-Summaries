---
title: 'GitHub Copilot For App Modernization'
layout: default
nav_order: 27
parent: 'Lab summaries'
---

**ID** 199388
**Number:** 43-514-02
**Name:** GitHub Copilot For App Modernization
**CloudSubscriptionPoolName:** TechMastery - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

### Exercise Summary

**Exercise 1: Setup the Environment**
  - **Goal:** Prepare the lab environment and sign in to required tools and services.
  - **Actions:**
    - Log in to the lab VM and GitHub with provided credentials.
    - Open Visual Studio Code and configure GitHub Copilot and App Modernization extensions.
    - Preconfigure Git and verify Copilot chat functionality.
  - **Validation:** Able to access the project folder in VS Code; Copilot chat and extensions are signed in and functional.

**Exercise 2: Assess Your Java Application**
  - **Goal:** Evaluate the sample Java application's readiness for Azure migration.
  - **Actions:**
    - Use the GitHub Copilot App Modernization extension to run an automated assessment.
    - Review the generated assessment report and Cloud Readiness issues.
  - **Validation:** Assessment report is generated and issues are visible in the extension pane.

**Exercise 3: Migrate to Azure Database for PostgreSQL Flexible Server**
  - **Goal:** Migrate the application's database from PostgreSQL to Azure Database for PostgreSQL using managed identity.
  - **Actions:**
    - Select and run the migration task for PostgreSQL in the Cloud Readiness section.
    - Confirm and proceed with Copilot prompts to generate migration plan and code changes.
    - Review and accept the proposed code changes and migration summary.
  - **Validation:** Migration summary and updated code are present; changes are accepted in VS Code.

**Exercise 4: Migrate from AWS S3 to Azure Blob Storage**
  - **Goal:** Replace AWS S3 storage with Azure Blob Storage using managed identity.
  - **Actions:**
    - Run the storage migration task for AWS S3 in the assessment report.
    - Confirm Copilot prompts and review generated migration summary and code changes.
    - Accept and apply the changes in VS Code.
  - **Validation:** Migration summary and updated code for Azure Blob Storage are present and accepted.

**Exercise 5: Migrate from AMQP RabbitMQ to Azure Service Bus**
  - **Goal:** Replace RabbitMQ messaging with Azure Service Bus using managed identity.
  - **Actions:**
    - Run the messaging service migration task in the assessment report.
    - Confirm Copilot prompts and review generated migration summary and code changes.
    - Accept and apply the changes in VS Code.
  - **Validation:** Migration summary and updated code for Azure Service Bus are present and accepted.

**Exercise 6: Completion**
  - **Goal:** Finalize the migration and review outcomes.
  - **Actions:**
    - Review migration summary and plan files for details.
    - Reference documentation and resources for further learning.
  - **Validation:** All migration steps are completed; summary and plan files are available for review; lab completion is submitted for credit.
