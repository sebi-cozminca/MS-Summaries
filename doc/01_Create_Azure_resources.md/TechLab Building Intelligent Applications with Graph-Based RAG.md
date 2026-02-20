---
title: 'TechLab: Building Intelligent Applications with Graph-Based RAG'
layout: default
nav_order: 57
parent: 'Lab summaries'
---

**ID** 186397  
**Number:** LAB116  
**Name:** TechLab: Building Intelligent Applications with Graph-Based RAG  
**CloudSubscriptionPoolName:** LAB426 Recycling CSS Pool  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** TrialFabricUsers  

---

## Exercise Summary

**Part 1: Getting Started with AI on Azure PostgreSQL Flexible Server**
- **Goal:** Set up and connect to an Azure PostgreSQL flexible server, populate it with sample data, and enable AI extensions.
- **Actions:**
  - Clone the lab repository and connect to the PostgreSQL database using Cloud Shell and pgAdmin.
  - Populate the database with sample data and explore its structure.
  - Install and configure the azure_ai extension and set up Azure OpenAI connection settings.
  - Review and test the Azure OpenAI schema for embedding generation.
- **Validation:** Successful connection to the database, sample data is loaded, and AI extensions are installed and configured.

**Part 2: Using AI-driven Features in Postgres**
- **Goal:** Leverage AI and vector search capabilities in PostgreSQL for advanced querying and semantic search.
- **Actions:**
  - Perform pattern matching queries using ILIKE.
  - Install vector and pg_diskann extensions, add vector columns, and generate embeddings for data.
  - Create DiskANN vector index for efficient similarity search.
  - Execute semantic search queries using embeddings and cosine distance.
- **Validation:** Semantic search returns relevant results even when exact keywords are not present; vector index improves search performance.

**Part 3: How RAG Chatbot Accuracy Improves with Different Techniques**
- **Goal:** Explore and evaluate the impact of context and retrieval techniques on RAG chatbot accuracy.
- **Actions:**
  - Review the RAG architecture and workflow.
  - Interact with a sample RAG application and test queries.
  - Analyze citation graphs to assess the recall of vector search.
- **Validation:** Application returns contextually relevant legal cases; citation graph shows recall percentage for vector search.

**Part 4: Improving RAG Accuracy with Advanced Techniques - Reranking and GraphRAG**
- **Goal:** Enhance RAG accuracy using reranking algorithms and knowledge graph-based retrieval.
- **Actions:**
  - Understand and test reranker queries using Azure ML and BGE model.
  - Implement and run graph queries using Apache AGE extension for GraphRAG.
  - Compare results of vector search, reranker, and GraphRAG in the RAG application.
- **Validation:** Reranker and GraphRAG options retrieve a higher percentage of relevant cases; citation graphs and query results confirm improved accuracy.
