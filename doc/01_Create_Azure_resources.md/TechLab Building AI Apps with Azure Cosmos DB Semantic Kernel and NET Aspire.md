---
title: 'TechLab: Building AI Apps with Azure Cosmos DB, Semantic Kernel and .NET Aspire'
layout: default
nav_order: 56
parent: 'Lab summaries'
---

**ID** 186394
**Number:** LAB510
**Name:** TechLab: Building AI Apps with Azure Cosmos DB, Semantic Kernel and .NET Aspire
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Tech Mastery Catalog Lab Instruction Summary

## Exercise Summary

**Exercise: Setup and Run the Starter Web Application**
- **Goal:** Prepare the environment and verify the starter application builds and runs successfully.
- **Actions:**
  - Log in to the lab VM and Azure CLI.
  - Assign required Azure roles and permissions.
  - Build and run the .NET Aspire Blazor application locally.
  - Trust the HTTPS developer certificate and launch the Aspire dashboard.
- **Validation:** Application launches, dashboard is accessible, and test chat returns a placeholder response.

**Exercise: Implement the Semantic Kernel**
- **Goal:** Integrate Semantic Kernel to enable real AI completions using Azure OpenAI.
- **Actions:**
  - Add OpenAI chat completion extension to SemanticKernelService.
  - Update methods to generate completions and summaries using Semantic Kernel.
  - Refactor ChatService to use the new Semantic Kernel implementation.
- **Validation:** Application returns real AI-generated responses instead of placeholders.

**Exercise: Implement Chat History (Context Window)**
- **Goal:** Enable context-aware conversations by maintaining chat history.
- **Actions:**
  - Implement context window logic in CosmosDbService to retrieve recent chat messages.
  - Update ChatService to use the context window for completions.
- **Validation:** Follow-up questions receive contextually relevant answers; chat history is used in completions.

**Exercise: Implement the RAG Pattern**
- **Goal:** Enhance responses using Retrieval Augmented Generation (RAG) with vector search on product data.
- **Actions:**
  - Add OpenAI embeddings extension to SemanticKernelService.
  - Implement vector search using Semantic Kernel's Cosmos DB connector.
  - Update system prompts and completion logic to include RAG data.
  - Refactor ChatService to generate embeddings, perform vector search, and call RAG completion.
- **Validation:** AI assistant provides product-specific answers; vector search and RAG pattern are functional.

**Exercise: Implement a Semantic Cache**
- **Goal:** Reduce latency and cost by caching LLM completions using semantic similarity.
- **Actions:**
  - Implement vector-based cache query in CosmosDbService.
  - Update ChatService to check the cache before generating new completions and to store new completions.
  - Tune cache similarity threshold for optimal results.
- **Validation:** Repeated or similar prompts return cached responses instantly; cache hits are indicated in the UI.

**Bonus Exercise: Explore the .NET Aspire Dashboard**
- **Goal:** Use the .NET Aspire dashboard to monitor, trace, and debug the application.
- **Actions:**
  - Issue requests and observe traces, logs, and spans in the dashboard.
  - Analyze request flows, cache hits/misses, and Cosmos DB telemetry.
  - Review log configuration and structured logs for diagnostics.
- **Validation:** Dashboard displays traces and logs for all major operations; cache and LLM pipeline behavior is observable.
