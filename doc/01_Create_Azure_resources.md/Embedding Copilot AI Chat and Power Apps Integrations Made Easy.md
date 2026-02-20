---
title: 'Embedding Copilot: AI Chat and Power Apps Integrations Made Easy'
layout: default
nav_order: 23
parent: 'Lab summaries'
---

**ID** 208652  
**Number:** LAB 632  
**Name:** Embedding Copilot: AI Chat and Power Apps Integrations Made Easy  
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** CopilotStudio, Events GHE w/ Copilot  

---

## Exercise Summary

**Exercise 1: Review and Understand the Starter Project Structure**
- **Goal:** Familiarize with the Blazor Server web application foundation for Copilot Studio integration.
- **Actions:**
  - Explore the CopilotStudioClient project structure and run the starter app to verify the echo service.
  - Review backend service and Razor component organization.
- **Validation:**
  - Echo bot responds correctly in the chat UI; project structure is understood.

**Exercise 2: Create a Simple Copilot Studio Agent**
- **Goal:** Build and configure a Copilot Studio agent as the backend conversational engine.
- **Actions:**
  - Provision a development environment in Copilot Studio.
  - Create, configure, and publish a new agent with Microsoft authentication and web search enabled.
  - Test agent responses and ensure Dataverse integration is visible.
- **Validation:**
  - Agent is published, responds to queries, and is visible in the correct environment.

**Exercise 3: Configure App Registration to Access the Copilot Studio Agent**
- **Goal:** Register and configure an Azure AD application for secure agent access.
- **Actions:**
  - Register a new application in Microsoft Entra ID (Azure AD).
  - Add delegated permissions (User.Read, offline_access, CopilotStudio.Copilots.Invoke).
  - Configure authentication settings, redirect URIs, and create a client secret.
- **Validation:**
  - App registration is complete with correct permissions and authentication settings; client secret is generated and stored.

**Exercise 4: Implement Basic Authentication and Authorization in the Blazor App**
- **Goal:** Enable secure, identity-aware access to the Copilot Studio client.
- **Actions:**
  - Configure Microsoft Identity Web for OpenID Connect authentication and token acquisition.
  - Update appsettings.json with Copilot Studio and Azure AD details.
  - Add authentication and authorization middleware and protect chat routes.
- **Validation:**
  - Users are prompted to sign in; chat interface is protected and accessible only to authenticated users.

**Exercise 5: Implement a Basic Copilot Studio Client Using the Microsoft 365 Agents SDK**
- **Goal:** Connect the Blazor app to Copilot Studio using the Agents SDK for delegated authentication and chat.
- **Actions:**
  - Implement AuthTokenHandler to attach user tokens to outgoing requests.
  - Refactor CopilotStudioIChatClient to use CopilotClient and support streaming, metadata parsing, and activity handling.
  - Register all required services and handlers in Program.cs.
- **Validation:**
  - Authenticated users can chat with the Copilot Studio agent; streaming and message handling work as expected.

**Exercise 6: Implement Markdown Rendering and Streaming Responses**
- **Goal:** Enhance the chat client with Markdown support and real-time streaming.
- **Actions:**
  - Integrate Markdig for Markdown-to-HTML conversion in chat responses.
  - Update UI components to handle streaming updates and partial responses.
- **Validation:**
  - Assistant messages render Markdown correctly; streaming responses appear incrementally in the chat UI.

**Exercise 7: Add a Dataverse MCP Server and Adaptive Cards with Custom Input Parameters**
- **Goal:** Extend the Copilot Studio agent with Dataverse integration and Adaptive Card support.
- **Actions:**
  - Integrate a Dataverse-backed MCP server with the agent.
  - Implement Adaptive Cards for structured user input and handle responses in the chat client.
- **Validation:**
  - Users can interact with Adaptive Cards; Dataverse data is accessible through the agent.

**Exercise 8: Implement Cookie-Based Distributed Token Caching (Optional)**
- **Goal:** Securely persist authentication tokens using encrypted cookies.
- **Actions:**
  - Add distributed cache implementation for MSAL tokens using chunked, encrypted cookies.
  - Update authentication configuration to use cookie-based token storage.
- **Validation:**
  - Tokens persist across requests; users remain authenticated after page reloads.

**Exercise 9: Add a Copilot Control to a Canvas App and Customize with Copilot Studio**
- **Goal:** Embed a custom Copilot experience in a Power Platform Canvas App using low-code tools.
- **Actions:**
  - Add a Copilot control to a Canvas App and connect it to a Copilot Studio agent.
  - Customize Copilot behavior using Copilot Studio without modifying app UI or writing code.
- **Validation:**
  - Copilot control is embedded and functional in the Canvas App; users can interact with the agent across app screens.

**Lab Completion**
- **Goal:** Reinforce integration patterns and provide additional resources.
- **Actions:**
  - Review best practices, compare low-code and pro-code approaches, and explore further documentation and sample projects.
- **Validation:**
  - Participants understand integration tradeoffs and have access to resources for continued learning.
