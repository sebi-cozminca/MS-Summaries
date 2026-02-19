---
title: 'Governing AI Apps & Agents with AI Gateway in Azure API Management'
layout: default
nav_order: 29
parent: 'Lab summaries'
---

**ID** 205795
**Number:** LAB519
**Name:** Governing AI Apps & Agents with AI Gateway in Azure API Management
**CloudSubscriptionPoolName:** Microsoft Events 25 - MSLEARN CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

### Exercise Summary

**Exercise 1: Review Deployed Azure Resources**
  - **Goal:** Understand the Azure resources provisioned for AI Gateway governance.
  - **Actions:**
    - Log into Azure Portal and locate the lab-ai-gateway resource group.
    - Review deployed services: API Center, API Management (APIM), AI Foundry, Application Insights, Log Analytics, and others.
  - **Validation:** All required resources are present and accessible in the resource group.

**Exercise 2: Review Deployed Azure AI Foundry Models**
  - **Goal:** Verify and test the AI model deployment in Azure AI Foundry.
  - **Actions:**
    - Access the AI Foundry portal and review the gpt-4.1 model deployment.
    - Test the model in the playground and review code samples for API integration.
    - Ensure agent execution is available in the portal.
  - **Validation:** Model responds to prompts; agent features are accessible.

**Exercise 3: Create the Inference API to Control Token Usage**
  - **Goal:** Expose the AI Foundry model via APIM with token usage controls.
  - **Actions:**
    - Add a new API in APIM from the AI Foundry resource.
    - Configure base path, enable token rate limiting, and set up Application Insights for metrics.
    - Enable token usage headers and tracking.
  - **Validation:** Inference API is created with correct policies and settings.

**Exercise 4: Test the Inference API in the Azure Portal**
  - **Goal:** Validate API configuration and policies through the APIM portal.
  - **Actions:**
    - Review API design, policies, and security settings.
    - Enable diagnostics and logging for LLM messages.
    - Test the API operation and inspect HTTP responses, headers, and trace logs.
  - **Validation:** API returns expected responses; token limits and logging are functional.

**Exercise 5: Create an APIM Subscription (API Key)**
  - **Goal:** Enable secure API access using APIM subscriptions.
  - **Actions:**
    - Create a new subscription in APIM with an API key for all APIs.
    - Note the generated keys for use in client applications.
  - **Validation:** Subscription is created and keys are available for API access.

**Exercise 6: Test the Inference API in VS Code**
  - **Goal:** Validate API access and token policies from a client environment.
  - **Actions:**
    - Log in to Azure CLI and open the provided VS Code project.
    - Run Jupyter notebook cells to test the API using both the OpenAI SDK and direct HTTP calls.
    - Test token rate limiting by sending multiple requests and analyze results.
  - **Validation:** API responses are received; rate limiting and token headers behave as configured.

**Exercise 7: View Language Models Analytics**
  - **Goal:** Monitor and analyze LLM usage and token consumption.
  - **Actions:**
    - Use APIM Analytics and Log Analytics to review token metrics and logs.
    - Query LLM logs using KQL and explore dashboard visualizations.
  - **Validation:** Token usage and request analytics are visible and accurate in monitoring tools.

**Exercise 8: Create MCP Servers (from Existing API and MCP Server)**
  - **Goal:** Expose APIs and external MCP servers through APIM for secure access.
  - **Actions:**
    - Create MCP servers for existing APIs and external endpoints.
    - Configure JWT validation policies for secure access.
    - Test MCP server connectivity and tool execution using MCP Inspector.
  - **Validation:** MCP servers are accessible and enforce authentication as configured.

**Exercise 9: Enable Private MCP Registry (Using API Center)**
  - **Goal:** Register and expose MCP servers and APIs for discovery via API Center.
  - **Actions:**
    - Integrate APIM with API Center and synchronize APIs/MCP servers.
    - Deploy and configure the API Center Developer Portal for anonymous access.
    - Verify MCP server discovery and endpoint access in the portal.
  - **Validation:** APIs and MCP servers are discoverable in API Center; portal is accessible.

**Exercise 10: Execute an AI Foundry Agent Using MCP Tools**
  - **Goal:** Demonstrate agent execution and tool integration with MCP endpoints.
  - **Actions:**
    - Set the Weather MCP endpoint in the Jupyter notebook and execute the agent cell.
    - Review agent execution, thread logs, and tool call results in both VS Code and AI Foundry portal.
  - **Validation:** Agent runs successfully, tool calls are logged, and results are visible in the portal.

**Optional: Execute Additional Labs**
  - **Goal:** Explore advanced AI Gateway scenarios (load balancing, FinOps, LLM log streaming).
  - **Actions:**
    - Select and run additional Jupyter notebooks as desired.
  - **Validation:** Optional labs execute and produce expected outputs.
