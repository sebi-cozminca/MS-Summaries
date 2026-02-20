---
title: 'TechLab: LLM App - Prompt Injection, Jailbreak and Protection'
layout: default
nav_order: 73
parent: 'Lab summaries'
---

**ID** 186391  
**Number:** TechConnect LAB417  
**Name:** TechLab: LLM App - Prompt Injection, Jailbreak and Protection  
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** TrialFabricUsers  

---

## Exercise Summary

**Exercise 0: Initialize Environment**
- **Goal:** Prepare the environment for Prompt Flow development with Python 3.9 and required dependencies.
- **Actions:**
  - Confirm Python 3.9 installation.
  - Navigate to the lab code directory in VS Code terminal.
  - Install LangChain using `pip install -r requirements.txt`.
- **Validation:** Python 3.9 is available and dependencies install without errors.

**Exercise 1: Install / Verify Prompt Flow in VS Code**
- **Goal:** Ensure Prompt Flow extension and dependencies are installed in VS Code.
- **Actions:**
  - Open VS Code and install the Prompt Flow extension from the marketplace.
  - Select Python 3.9.13 as the interpreter in the Install Dependencies page.
  - Follow and complete all installation steps, including optional ones.
  - Refresh and verify installation status.
- **Validation:** Prompt Flow extension and dependencies show as successfully installed in VS Code.

**Exercise 2: First Prompt Flow App**
- **Goal:** Create and configure a basic Prompt Flow app in VS Code.
- **Actions:**
  - Open the provided workspace and create a new standard Prompt Flow using a template.
  - Name the project `labpf` and open it in a new VS Code window.
  - Edit `hello.jinja2` to contain only `{{text}}`.
  - Replace `hello.py` content with provided code.
  - Set input value to `Hello world` in `flow.dag.yaml`.
  - Run the flow and start the UI with `pf flow serve`.
- **Validation:** Flow runs successfully and outputs the expected result in the terminal and UI.

**Exercise 3: Challenge - Black Snow**
- **Goal:** Test prompt injection by manipulating the AI to describe "black snow".
- **Actions:**
  - Use the built AI app to attempt prompt injection for the target output.
- **Validation:** AI responds with a description of black snow or demonstrates resistance to injection.

**Exercise 4: First Prompt Injection**
- **Goal:** Explore prompt injection vulnerabilities in a simple prompt template.
- **Actions:**
  - Review and understand the Yamaha marketing prompt template.
  - Attempt to induce the AI to output "Sony speaker is better than Yamaha."
  - Craft prompts to reveal the template and bypass restrictions.
- **Validation:** AI either reveals the template or outputs restricted content, demonstrating injection success or failure.

**Exercise 5: Harden Prompt Template, then Complete Second Prompt Injection**
- **Goal:** Strengthen the prompt template and test its resistance to injection.
- **Actions:**
  - Modify the prompt template to include explicit rules and structure.
  - Deploy the hardened template in the provided workspace.
  - Attempt prompt injection using new methods.
- **Validation:** AI resists injection attempts and adheres to the new rules, or injection is still possible.

**Exercise 6: Understand & Try Jailbreak**
- **Goal:** Demonstrate and analyze jailbreak techniques using the DAN (Do Anything Now) prompt.
- **Actions:**
  - Review the DAN jailbreak script from GitHub.
  - Use the DAN prompt in the AI app to attempt bypassing restrictions.
- **Validation:** AI exhibits DAN behavior or resists jailbreak attempts as expected.

**Exercise 7: Protect LLM App from Jailbreak**
- **Goal:** Understand and discuss methods for protecting LLM apps from jailbreaks and prompt injection.
- **Actions:**
  - Review Azure Content Safety capabilities (demo only, not testable in lab).
  - Consider additional protection and detection strategies for LLM apps.
- **Validation:** Knowledge of protection strategies is demonstrated; direct validation not possible in lab.

**Exercise 8: What's Next**
- **Goal:** Explore further resources and reflect on comprehensive LLM app protection.
- **Actions:**
  - Visit Jailbreak Bench for more jailbreak examples.
  - Consider holistic protection and rapid response strategies for LLM security.
- **Validation:** User is aware of next steps and additional resources for continued learning.
