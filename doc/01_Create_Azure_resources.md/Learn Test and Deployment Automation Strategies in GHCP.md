---
title: 'Learn Test and Deployment Automation Strategies in GHCP'
layout: default
nav_order: 33
parent: 'Lab summaries'
---

**ID** 205273
**Number:** LAB 334
**Name:** Learn Test and Deployment Automation Strategies in GHCP
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

# Exercise Summary

**Exercise 1: Prerequisites Installation/Verification**
- **Goal:** Set up the development environment and required tools for AKS deployment and testing with GitHub Copilot.
- **Actions:**
  - Verify GitHub Copilot is available and active in VS Code.
  - Use Copilot to install Azure CLI and kubectl, and verify Git installation.
  - Clone the lab repository using Copilot.
  - Authenticate to Azure using Azure CLI and set the correct subscription.
- **Validation:**
  - Azure CLI, kubectl, and Git are installed and configured; authenticated to Azure; Copilot is ready.

**Exercise 2: Verify Azure Resources Setup**
- **Goal:** Connect to pre-provisioned Azure resources and configure kubectl for AKS access.
- **Actions:**
  - Log in to the Azure Portal and locate the "TechConnect2026" resource group and AKS cluster.
  - Use Copilot to retrieve AKS credentials and configure kubectl.
  - Verify AKS connectivity by listing cluster nodes.
- **Validation:**
  - kubectl is configured and able to access the AKS cluster; nodes are in "Ready" state.

**Exercise 3: Deploy Application to AKS using GitHub Copilot**
- **Goal:** Deploy a four-microservice application to AKS and verify deployment status.
- **Actions:**
  - Navigate to the manifest directory in the cloned repo.
  - Use Copilot to deploy the application using the provided YAML manifest.
  - Monitor pod status and verify all pods are running.
  - Check Kubernetes services and obtain the external IP for the store-front service.
- **Validation:**
  - Application is deployed; all pods are running; services are created; LoadBalancer external IP is provisioned.

**Exercise 4: Automated Testing - Verify Deployment and Get Application URL**
- **Goal:** Validate application deployment and access the running web application.
- **Actions:**
  - Use Copilot to retrieve the external IP of the store-front service.
  - Access the application in a browser and test core features (browse, add to cart, place order).
- **Validation:**
  - Application homepage is accessible; all features function as expected.

**Exercise 5: Functional Testing**
- **Goal:** Generate functional test cases for user stories using Copilot.
- **Actions:**
  - Open the solution folder and switch Copilot Chat to Agent Mode.
  - Prompt Copilot to design functional test cases for a user story, attaching required files.
  - Review generated test cases in CSV and JSON formats.
- **Validation:**
  - Functional test cases are generated and saved in the designated folder.

**Exercise 6: Test Automation Using Playwright MCP Server**
- **Goal:** Create automation test scripts for the application using Playwright MCP Server.
- **Actions:**
  - Ensure Playwright MCP Server is configured in Copilot Tools.
  - If needed, add Playwright configuration and install Chrome.
  - Prompt Copilot to generate Playwright automation scripts using the functional test cases and instructions.
  - Allow all permissions requested by the Agent.
- **Validation:**
  - Playwright automation scripts are generated and available for execution.

**Lab Completion**
- **Goal:** Master test automation and deployment validation using GitHub Copilot Agent Mode.
- **Actions:**
  - Complete all exercises, review troubleshooting tips, and explore next steps for advanced testing and CI/CD integration.
- **Validation:**
  - All lab objectives are met; user is able to automate deployment, testing, and validation workflows for AKS applications using Copilot.