---
title: 'Multi-Agent Apps with Microsoft Agent Framework or LangGraph'
layout: default
nav_order: 40
parent: 'Lab summaries'
---

**ID** 207066
**Number:** LAB518
**Name:** Multi-Agent Apps with Microsoft Agent Framework or LangGraph
**CloudSubscriptionPoolName:** Microsoft Events 25 - MSLEARN CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Exercise Summary: Multi-Agent Apps with Microsoft Agent Framework or LangGraph

## C# Track: Microsoft Agent Framework (Semantic Kernel Agents)

**Exercise 0: Configure Local Lab Resources**
- **Goal:** Set up Azure resources and verify lab environment readiness.
- **Actions:**
  - Log into Azure Portal and locate the resource group.
  - Confirm all resources are deployed.
  - Start backend and frontend apps in VS Code.
- **Validation:** Azure resources visible; backend and frontend apps start without errors.

**Exercise 1: Creating Your First Agent**
- **Goal:** Build a basic conversational agent using Microsoft Agent Framework and Azure OpenAI.
- **Actions:**
  - Instantiate the agent framework and configure Azure OpenAI client.
  - Implement a simple chat agent with greeting and translation capabilities.
  - Integrate agent response handling in the chat service.
- **Validation:** App compiles; agent responds and translates user input as expected.

**Exercise 2: Connecting Agents to Memory**
- **Goal:** Enable persistent chat history and context using Azure Cosmos DB.
- **Actions:**
  - Integrate Cosmos DB for session and message storage.
  - Update agent and chat service to persist and retrieve conversation history.
  - Test context-aware responses across multiple turns.
- **Validation:** Agent maintains context; chat history is stored and retrievable from Cosmos DB.

**Exercise 3: Agent Specialization**
- **Goal:** Implement specialized agents with domain-specific tools and prompts.
- **Actions:**
  - Define banking domain models and CRUD functions.
  - Create specialized agents (Coordinator, Customer Support, Sales, Transactions) with unique prompts and tools.
  - Integrate vector search with Azure Cosmos DB for product recommendations.
  - Dynamically build agents and assign tools.
- **Validation:** Each agent responds according to its role; vector search and tool functions operate correctly.

**Exercise 4: Multi-Agent Orchestration**
- **Goal:** Coordinate multiple agents using orchestration strategies and automated agent selection.
- **Actions:**
  - Implement agent selection and termination strategies using prompt templates.
  - Define structured response formats for agent routing.
  - Replace single-agent workflow with group chat orchestration.
  - Test dynamic agent selection and multi-agent collaboration.
- **Validation:** Agent selection is dynamic; agents invoke correct tools; orchestration logs and debug outputs are accurate.

**Exercise 5: MCP Integration**
- **Goal:** Extend agent capabilities by integrating external Model Context Protocol (MCP) server tools.
- **Actions:**
  - Configure MCP client and authenticate with external MCP server.
  - Update agent factory and services to use MCP tools.
  - Test agent-to-MCP server communication and tool invocation.
  - Enable MCP as the preferred tool source in configuration.
- **Validation:** Agents dynamically load and use MCP tools; agent selection and tool invocation work as expected; MCP server logs show successful integration.

---

## Python Track: LangGraph (LangChain Agents)

**Exercise 0: Configure Local Lab Resources**
- **Goal:** Prepare Azure and local environment for the lab.
- **Actions:**
  - Log into Azure Portal and verify resource group deployment.
  - Set up Python virtual environment and install dependencies.
  - Start backend (FastAPI) and frontend (Angular) applications.
- **Validation:** Backend and frontend start without errors; resources visible in Azure.

**Exercise 1: Creating Your First Agent**
- **Goal:** Build a simple LangGraph agent with prompt-driven behavior.
- **Actions:**
  - Define agent prompts in separate files.
  - Create a coordinator agent using `create_react_agent`.
  - Implement agent and human nodes in a LangGraph state graph.
  - Wire up API layer for frontend integration.
- **Validation:** Agent responds to user input; API returns expected responses.

**Exercise 2: Connecting Agents to Memory**
- **Goal:** Add persistent state and chat history using Azure Cosmos DB.
- **Actions:**
  - Integrate CosmosDBSaver as a checkpointer for agent state.
  - Store and retrieve chat history and agent state in Cosmos DB.
  - Implement deterministic agent routing using the "active agent" field.
- **Validation:** Agent state and chat history persist across sessions; routing is consistent.

**Exercise 3: Agent Specialization**
- **Goal:** Create multiple specialized agents with domain-specific tools and prompts.
- **Actions:**
  - Define and register tools for sales, transactions, and support agents.
  - Implement vector search for product recommendations using Azure Cosmos DB.
  - Update agent prompts to guide tool usage and agent transfers.
  - Test agent collaboration and tool invocation.
- **Validation:** Specialized agents perform correct actions; vector search and tool calls succeed; chat history reflects agent transfers.

**Exercise 4: Multi-Agent Orchestration**
- **Goal:** Enable agent-to-agent communication and collaborative workflows.
- **Actions:**
  - Update agent tools to allow inter-agent transfers.
  - Implement agent tracing and monitoring with LangSmith.
  - Add environment variables for tracing and monitoring.
  - Test agent collaboration and monitor traces in LangSmith.
  - Expose API endpoints for automated and manual testing (Swagger UI).
- **Validation:** Agents transfer tasks as needed; traces appear in LangSmith; API endpoints function as expected.

**Exercise 5: Converting to Model Context Protocol (MCP)**
- **Goal:** Refactor agents to use MCP for tool discovery and invocation.
- **Actions:**
  - Update agent code to load tools from an MCP server using `langchain_mcp_adapters`.
  - Configure MCP client authentication and session management.
  - Start and test the MCP server independently.
  - Test the complete MCP-enabled system via API and frontend.
  - Use VS Code MCP client for direct tool interaction.
- **Validation:** Agents dynamically load and invoke MCP tools; system operates with MCP server; VS Code MCP client connects and lists tools.

---

### Validation (General)
- Successful agent responses and tool invocations.
- Persistent chat history and agent state in Cosmos DB.
- Dynamic agent selection and orchestration.
- MCP integration confirmed by tool discovery and usage.
- Tracing and monitoring data available in LangSmith (Python track).
- API and frontend tests pass with expected outputs.
