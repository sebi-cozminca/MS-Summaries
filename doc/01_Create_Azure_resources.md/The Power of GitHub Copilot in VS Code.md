---
title: 'The Power of GitHub Copilot in VS Code'
layout: default
nav_order: 89
parent: 'Lab summaries'
---

**ID** 205601
**Number:** LAB510
**Name:** The Power of GitHub Copilot in VS Code
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

# Exercise Summary

**Exercise 1: Environment Setup and Copilot Configuration**
- **Goal:** Prepare the lab environment and configure GitHub Copilot in Visual Studio Code.
- **Actions:**
  - Log into the provided virtual machine.
  - Access and reset Temporary Access Password (TAP) if needed.
  - Open Visual Studio Code and initiate Copilot login via the chat interface.
  - Authenticate using provided credentials and authorize VS Code access.
  - Confirm Copilot setup by verifying the welcome tab in VS Code.
- **Validation:**
  - Copilot welcome tab is visible in VS Code, confirming successful setup.

**Exercise 2: Clone Lab Repository**
- **Goal:** Obtain the lab codebase for hands-on exercises.
- **Actions:**
  - Open the Source Control panel in VS Code.
  - Clone the repository from `https://github.com/github-samples/pets-workshop`.
  - Select the destination folder and open the cloned repository in VS Code.
- **Validation:**
  - Repository is opened and visible in VS Code workspace.

**Exercise 3: Start the Application**
- **Goal:** Launch the backend and frontend applications for the lab.
- **Actions:**
  - Open a new terminal in VS Code.
  - Run the startup script: `./scripts/start-app.ps1`.
  - Wait for dependencies to install and both backend (Flask) and frontend (Astro/Svelte) apps to start.
  - Access backend at `http://localhost:5100/api/dogs` and frontend at `http://localhost:4321`.
- **Validation:**
  - Both URLs are accessible and display the expected content.

**Exercise 4: Add a New Endpoint to the Server**
- **Goal:** Extend the backend API with a new endpoint.
- **Actions:**
  - Follow linked instructions to implement and test a new API endpoint in the Flask backend.
- **Validation:**
  - New endpoint is accessible and returns correct data.

**Exercise 5: Explore the Project**
- **Goal:** Understand the structure and components of the lab project.
- **Actions:**
  - Review project files and architecture as guided by the linked instructions.
- **Validation:**
  - Key components and their roles are identified and understood.

**Exercise 6: Cloudify the Backend**
- **Goal:** Integrate cloud capabilities into the backend application.
- **Actions:**
  - Follow linked instructions to update backend for cloud integration.
- **Validation:**
  - Backend demonstrates cloud-enabled features as described.

**Exercise 7: Interact with Azure Using Natural Language**
- **Goal:** Enable natural language interaction with Azure services.
- **Actions:**
  - Implement and test natural language features as per linked instructions.
- **Validation:**
  - Successful interaction with Azure services using natural language queries.

**Exercise 8: Using the MSSQL Extension for Visual Studio Code**
- **Goal:** Work with SQL Server databases in VS Code using the MSSQL extension.
- **Actions:**
  - Install and configure the MSSQL extension.
  - Connect to SQL Server and perform guided database tasks.
- **Validation:**
  - Database operations complete successfully in VS Code.

**Exercise 9: Accelerating Infrastructure as Code (IaC) with GitHub Copilot**
- **Goal:** Leverage Copilot to streamline IaC development.
- **Actions:**
  - Use Copilot to generate and refine infrastructure code as per instructions.
- **Validation:**
  - Infrastructure code is generated and validated as functional.

**Bonus Lab 1: Add Filter Feature with Copilot Edits**
- **Goal:** Enhance the dog list page with breed filtering and availability options.
- **Actions:**
  - Use Copilot Edits mode to update both Flask backend and Svelte frontend for filtering features.
- **Validation:**
  - Dog list page supports filtering by breed and availability.

**Bonus Lab 2: Add Themes with Copilot Agent Mode**
- **Goal:** Implement a theming system for the Tailspin Shelter website using Copilot Agent mode.
- **Actions:**
  - Allow Copilot Agent to autonomously plan and add theming support across the project.
- **Validation:**
  - Theming system is present and functional on the website.

**Lab Completion and Survey**
- **Goal:** Finalize the lab and submit completion data.
- **Actions:**
  - Complete the end-of-lab survey and submit results for credit.
- **Validation:**
  - Survey is submitted and lab completion is recorded for credit.