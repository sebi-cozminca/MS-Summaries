---
title: 'TechLab: AI Agents in Action: Transforming through Automation and Intelligence'
layout: default
nav_order: 51
parent: 'Lab summaries'
---

**ID** 186390  
**Number:** TechConnect Lab114  
**Name:** TechLab: AI Agents in Action: Transforming through Automation and Intelligence  
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Environment and Azure Portal Login**
- **Goal:** Access the lab environment and Azure portal with the required credentials.
- **Actions:**
  - Log in to the provided virtual machine using the supplied password.
  - Open Edge browser and sign in to the Azure portal with the given username and access token.
- **Validation:**
  - Successful access to both the VM and Azure portal.

**Exercise 2: Grant OpenAI Permission**
- **Goal:** Assign the Azure AI Developer role to the lab user for agent creation.
- **Actions:**
  - In the Azure portal, navigate to the Azure AI Foundry resource in the agents-lab resource group.
  - Use Access control (IAM) to add the Azure AI Developer role to the lab user.
- **Validation:**
  - User is listed with the Azure AI Developer role in the resource's access control panel.

**Exercise 3: Update Notebooks**
- **Goal:** Ensure the latest version of lab notebooks is available in the environment.
- **Actions:**
  - Open Windows Terminal and configure the Git safe directory.
  - Navigate to the Lab Files directory and run `git pull` to update notebooks.
- **Validation:**
  - Git output confirms notebooks are up to date.

**Exercise 4: Open and Run Notebooks**
- **Goal:** Set up and execute lab notebooks in Visual Studio Code.
- **Actions:**
  - Open the Lab Files directory in VS Code and select the setup notebook.
  - Choose the pre-installed Python kernel and execute the setup notebook.
  - Select and run additional lab notebooks as desired, each focusing on different agent capabilities (basics, models, grounding, actions, monitoring, multi-agent, bonus).
- **Validation:**
  - Notebooks execute successfully; each lab can be run independently and produces expected outputs.
