---
title: 'Next-Gen AKS Operations with Models, and Agents, and MCPs (oh my!)'
layout: default
nav_order: 41
parent: 'Lab summaries'
---

**ID** 205503
**Number:** LAB517
**Name:** Next-Gen AKS Operations with Models, and Agents, and MCPs (oh my!)
**CloudSubscriptionPoolName:** Ignite 2025 - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

# Exercise Summary

**Exercise 1: Environment Preparation**
- **Goal:** Set up and authenticate the lab environment for AKS operations with AI agents.
- **Actions:**
  - Log into Azure Portal and verify access to pre-provisioned resources.
  - Connect to the AKS cluster using Azure CLI and kubectl.
  - Run setup script to deploy required Kubernetes resources.
  - Authenticate GitHub Copilot in VS Code and ensure WSL remote connection is active.
- **Validation:**
  - Confirm Azure Portal access, kubectl connectivity, successful setup script completion, and Copilot authentication.

**Exercise 2: Explore AKS MCP Server with GitHub Copilot**
- **Goal:** Interact with the AKS MCP server using GitHub Copilot to discover available tools and cluster information.
- **Actions:**
  - Start the AKS MCP server in VS Code.
  - Use Copilot Chat to list available MCP tools and query AKS cluster status and health.
- **Validation:**
  - Copilot lists MCP tools and provides accurate cluster diagnostics.

**Exercise 3: CLI Agent for AKS**
- **Goal:** Use the CLI Agent for AKS to troubleshoot and plan cluster operations via natural language.
- **Actions:**
  - Configure the CLI Agent to use Azure AI Foundry models.
  - Start an agent session and query available tools and slash commands.
  - Request Kubernetes version, available upgrades, and run pre-upgrade checks.
  - Generate a full upgrade runbook and monitoring plan.
- **Validation:**
  - Agent provides upgrade compatibility analysis and actionable upgrade plan.

**Exercise 4: kagent with Azure**
- **Goal:** Deploy and interact with kagent as a Kubernetes-native AI agent platform.
- **Actions:**
  - Access the kagent dashboard and verify deployment.
  - Interact with the k8s-agent to query cluster resources, logs, and best practices.
  - Test prompts for high availability, resource management, and image best practices.
- **Validation:**
  - kagent dashboard is accessible and agents respond with accurate cluster insights.

**Exercise 5: Integrate AKS MCP Server with kagent**
- **Goal:** Connect kagent agents to the AKS MCP server for enhanced AKS operations.
- **Actions:**
  - Verify AKS MCP server deployment in the cluster.
  - Create a RemoteMCPServer resource in kagent for the AKS MCP server.
- **Validation:**
  - kagent agents can access AKS MCP tools and confirm server readiness.

**Exercise 6: Deploy and Test Specialized AKS Agent**
- **Goal:** Deploy a specialized AKS agent with deep Azure and Kubernetes expertise.
- **Actions:**
  - Apply the AKS agent manifest via kubectl.
  - Verify agent readiness and tool access.
  - Interact with the agent in the kagent dashboard to test AKS-specific queries and diagnostics.
- **Validation:**
  - Agent is ready, exposes AKS MCP tools, and responds to operational queries.

**Exercise 7: Build and Validate Multi-Agent System**
- **Goal:** Enable multi-agent collaboration by connecting the AKS agent to other specialized agents.
- **Actions:**
  - Edit the AKS agent to add k8s-agent and cilium-policy-agent as collaborators.
  - Validate tool configuration and test delegation with network policy and deployment analysis prompts.
- **Validation:**
  - AKS agent delegates tasks to specialized agents and provides collaborative troubleshooting.

**Exercise 8 (Optional): AI-Driven Troubleshooting Scenarios**
- **Goal:** Demonstrate AI-powered automation for real-world AKS operational scenarios.
- **Actions:**
  - Orchestrate load testing and monitor autoscaling with AI agents.
  - Diagnose and remediate node health issues using conversational commands.
  - Perform proactive cluster health assessments with multi-agent diagnostics.
- **Validation:**
  - Agents provide actionable insights, automate troubleshooting, and validate successful remediation or optimization.
