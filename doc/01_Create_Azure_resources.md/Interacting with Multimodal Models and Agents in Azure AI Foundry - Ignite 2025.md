---
title: 'Interacting with Multimodal Models and Agents in Azure AI Foundry - Ignite 2025'
layout: default
nav_order: 31
parent: 'Lab summaries'
---

**ID** 205277
**Number:** LAB512
**Name:** Interacting with Multimodal Models and Agents in Azure AI Foundry - Ignite 2025
**CloudSubscriptionPoolName:** Ignite 2025 - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

### Exercise Summary

**Exercise 1: Get Started**
  - **Goal:** Set up the lab environment and access the required tools.
  - **Actions:**
    - Log in to the lab VM and GitHub Codespaces with provided credentials.
    - Launch the workshop codespace and sign in to Azure and GitHub in VS Code.
    - Verify installation of AI Toolkit and Azure AI Foundry extensions.
  - **Validation:** Codespace is running in VS Code with all required extensions and access to the lab project.

**Exercise 2: Model Selection**
  - **Goal:** Discover, filter, and compare AI models for multimodal agent prototyping.
  - **Actions:**
    - Use the AI Toolkit Model Catalog to filter models by provider, publisher, and features.
    - Add selected models (e.g., OpenAI GPT-5-mini, Mistral Small 3.1) to your collection.
    - Test and compare models in the Playground using text and image prompts.
    - Analyze outputs for quality, detail, speed, and token usage.
    - Import the selected model from Microsoft Foundry for further use.
  - **Validation:** Models are added, tested, and compared; a suitable model is selected and available in the Playground.

**Exercise 3: Model Augmentation**
  - **Goal:** Enhance model performance and relevance using prompt engineering and context data.
  - **Actions:**
    - Craft a clear and context-rich system message to guide model behavior.
    - Test the model with multimodal prompts (text and images) and validate adherence to instructions.
    - Attach grounding data (e.g., product catalog JSON) to provide business context.
    - Evaluate model responses for relevance and accuracy using the attached data.
  - **Validation:** Model generates context-aware, relevant responses; grounding data is correctly referenced in outputs.

**Exercise 4: Agent Building**
  - **Goal:** Prototype a multimodal agent using Agent Builder and integrate external tools.
  - **Actions:**
    - Use Agent Builder to define agent name, model, instructions, and tools.
    - Start the MCP server and add the relevant tool (e.g., get_products_by_name) to the agent.
    - Test the agent with multimodal prompts and verify tool invocation and output.
  - **Validation:** Agent responds to prompts, invokes tools as needed, and provides grounded recommendations.

**Exercise 5: Migrate to Code**
  - **Goal:** Export the agent prototype to code for integration and deployment.
  - **Actions:**
    - Use Agent Builder to generate code in the preferred SDK and language (e.g., Python with Microsoft Agent Framework).
    - Review and update generated code, replacing placeholders as needed.
    - Optionally, run the code and use GitHub Copilot Chat for code understanding and UI integration.
  - **Validation:** Code is generated, reviewed, and ready for integration; agent logic is preserved in the exported script.

**Exercise 6: Bonus - Manual Evaluation**
  - **Goal:** Systematically evaluate agent responses for quality and relevance.
  - **Actions:**
    - Add variables to agent instructions and create evaluation datasets (manual, generated, or imported).
    - Run evaluations and manually rate outputs with thumbs up/down based on accuracy and usefulness.
  - **Validation:** Evaluation results are recorded; agent performance is assessed across different contexts.

**Exercise 7: Summary and Next Steps**
  - **Goal:** Review key learnings and understand best practices for production deployment.
  - **Actions:**
    - Summarize the process from model selection to agent deployment.
    - Review recommendations for using Azure-hosted models, evaluation, monitoring, and continuous improvement.
  - **Validation:** Best practices and next steps are understood; agent is ready for further development or deployment.
