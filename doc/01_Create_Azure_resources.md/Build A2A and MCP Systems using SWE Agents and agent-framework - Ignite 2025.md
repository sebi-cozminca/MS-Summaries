---
title: 'Build A2A and MCP Systems using SWE Agents and agent-framework - Ignite 2025'
layout: default
nav_order: 6
parent: 'Lab summaries'
---

**ID** 205281  
**Number:** LAB513
**Name:** Build A2A and MCP Systems using SWE Agents and agent-framework - Ignite 2025  
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** Events GHE w/ Copilot  

---

## Exercise Summary

**Lab Environment Setup**
- **Goal:** Prepare the Skillable Lab Cloud VM and required tools for agent-framework development.
- **Actions:**
  - Enter fullscreen mode in the Skillable Lab Cloud VM and confirm you are not using the Surface laptop.
  - Sign in with provided credentials.
  - Verify pre-installed tools: VS Code, Python 3.12, uv, Azure CLI, azd, AI Toolkit, Microsoft Foundry extension, and Git.
- **Validation:**
  - All work is performed in the browser-based VM; required tools are available and accessible.

**Clone and Set Up the Repository**
- **Goal:** Obtain and prepare the agent-framework codebase for development.
- **Actions:**
  - Clone the Microsoft spec-to-agents repository and check out the ignite-2025 branch.
  - Open the project in VS Code and trust the workspace.
  - Install dependencies using `uv sync` in the integrated terminal.
- **Validation:**
  - Repository is cloned, branch is set, and dependencies are installed without errors.

**Start Azure Resource Provisioning (Background Process)**
- **Goal:** Provision all required Azure resources for agent deployment and testing.
- **Actions:**
  - Authenticate with Azure Developer CLI (`azd auth login`) and Azure CLI (`az login --use-device-code`).
  - Create a new azd environment and start provisioning resources with `azd provision`.
- **Validation:**
  - Azure authentication is successful; provisioning runs in the background while coding continues.

**Understand the Codebase Structure**
- **Goal:** Familiarize with the organization and responsibilities of the agent-framework codebase.
- **Actions:**
  - Review the structure and purpose of key folders: agents, prompts, tools, models, workflow, utils, config, container, main.py, and console.py.
- **Validation:**
  - User understands where to implement and find agent logic, tools, orchestration, and configuration.

**Exercise 1: Create Your First Agent**
- **Goal:** Implement a Venue Specialist agent with web search and optional MCP tool capabilities.
- **Actions:**
  - Edit `venue_specialist.py` to initialize agent tools, add web search and sequential-thinking MCP tool if available, and create the agent with structured output.
- **Validation:**
  - Agent creation code is complete and ready for workflow integration.

**Exercise 2: Implement a Web Search Tool**
- **Goal:** Provide agents with Bing-powered web search capability via a custom tool.
- **Actions:**
  - Implement the `web_search` tool in `bing_search.py` using HostedWebSearchTool and a temporary agent pattern.
  - Ensure proper async context management and error handling.
- **Validation:**
  - Tool implementation is complete; agents can invoke web search as needed.

**Exercise 3: Add MCP Sequential Thinking Tool**
- **Goal:** Integrate the MCP sequential-thinking tool for advanced reasoning in agents.
- **Actions:**
  - Implement MCP tool creation in `mcp_tools.py` using MCPStdioTool and return as a dictionary for dependency injection.
- **Validation:**
  - MCP tool is available for agents and managed by the framework lifecycle.

**Exercise 4: Define Structured Output Format**
- **Goal:** Enforce predictable, parseable agent responses using Pydantic models.
- **Actions:**
  - Define the `SpecialistOutput` model in `messages.py` with fields for summary, next_agent, user_input_needed, and user_prompt.
- **Validation:**
  - Agents return structured JSON outputs, enabling reliable workflow routing and user interaction.
