---
title: 'TechLab: Guardians of Innovation: Establishing Security Baselines for ML/AI'
layout: default
nav_order: 69
parent: 'Lab summaries'
---

**ID** 186399
**Number:** LAB418
**Name:** TechLab: Guardians of Innovation: Establishing Security Baselines for ML/AI
**CloudSubscriptionPoolName:** Microsoft Event Subscription (CSS)
**AllowSave:** False
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise Blank Admin Only 15S (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

# TechLab Guardians of Innovation: Establishing Security Baselines for MLAI – Lab Instruction Summary

## Exercise Summary

**Exercise 1: Introduction to the Lab Guide**
- **Goal:** Understand the importance of securing infrastructure in MLOps projects using Azure MLOps (v2) Solution Accelerator.
- **Actions:**
  - Review lab objectives and provided reference links.
  - Note the importance of using standard templates and configurations.
- **Validation:** Ready to proceed to environment setup after reading.

**Exercise 2: Setup Azure DevOps Environment**
- **Goal:** Prepare Azure DevOps for code repository and pipeline deployment.
- **Actions:**
  - Sign in to Azure DevOps and rename the default project.
  - Verify Microsoft-hosted parallel jobs are enabled in organization settings.
- **Validation:** Project renamed and parallel jobs confirmed enabled.

**Exercise 3: Create Service Principal**
- **Goal:** Create a service principal for Azure DevOps to access Azure resources securely.
- **Actions:**
  - Log in to Azure Portal and launch Cloud Shell (Bash).
  - Run provided Bash commands to create a service principal with Contributor role.
  - Save generated appID, displayName, password, and tenant values for later use.
- **Validation:** Service principal credentials are saved and ready for Azure DevOps configuration.

**Exercise 4: Assign Service Principal to Azure DevOps Project**
- **Goal:** Configure Azure DevOps to use the created service principal for resource access.
- **Actions:**
  - Add a new Azure Resource Manager service connection in Azure DevOps.
  - Input service principal credentials and subscription details.
  - Grant access permission to all pipelines and verify connection.
- **Validation:** Service connection is verified and saved in Azure DevOps.

**Exercise 5: Set Up Source Repository with Azure DevOps**
- **Goal:** Import and configure the source code repository for the project.
- **Actions:**
  - Import the GitHub repository (Azure/mlops-v2-ado-demo) into Azure DevOps.
  - Adjust repository and pipeline security permissions for the Build Service user.
- **Validation:** Repository imported and permissions set for build and pipeline operations.

**Exercise 6: Deploying Infrastructure via Azure DevOps**
- **Goal:** Deploy MLOps infrastructure using Azure DevOps pipelines.
- **Actions:**
  - Edit the config-infra-prod.yml file with specified namespace, postfix, and location.
  - Commit changes and create a new pipeline using the provided YAML file.
  - Run the pipeline and grant required permissions when prompted.
- **Validation:** Pipeline completes successfully, deploying resource group, storage, container registry, Application Insights, Key Vault, AML workspace, and compute cluster.

**Exercise 7: Enable Defender for Cloud Features**
- **Goal:** Enhance security posture by enabling Microsoft Defender for Cloud.
- **Actions:**
  - Enable Defender CSPM in Azure Portal for the subscription.
  - Add Azure DevOps as an environment in Defender for Cloud and authorize access.
- **Validation:** Defender for Cloud is enabled and Azure DevOps is connected; resources will appear in inventory and security pages.

**Exercise 8: Review Defender for Cloud Recommendations**
- **Goal:** Review security recommendations for the deployed environment.
- **Actions:**
  - Access Security Posture in Defender for Cloud.
  - View recommendations for the subscription.
- **Validation:** Recommendations are visible for review and action.

**Exercise 9: Tighten Up Security**
- **Goal:** Improve security by updating service connection authentication.
- **Actions:**
  - Create a new Azure Resource Manager service connection using workload identity federation.
  - Update config-infra-prod.yml to use the new service connection if needed.
- **Validation:** New service connection is created and ready for use.

**Exercise 10: Additional Security Controls (Best Practices)**
- **Goal:** Understand and plan for advanced security controls in MLOps projects.
- **Actions:**
  - Review recommendations for using virtual networks, disabling public network access, enabling resource logs, and securing Key Vault with firewalls.
- **Validation:** Awareness of best practices; not implemented in this lab but recommended for production.

**Exercise 11: Manage Access and RBAC**
- **Goal:** Understand access management and RBAC for Azure Machine Learning workspaces.
- **Actions:**
  - Review built-in roles and managed identity permissions for AML workspaces.
  - Learn about restricting access and restoring managed identity permissions if needed.
- **Validation:** Knowledge of RBAC roles and managed identity usage for secure access control.

**Exercise 12: Lab Completion**
- **Goal:** Complete the lab and submit for credit.
- **Actions:**
  - Answer survey questions and select "Submit" to record completion.
- **Validation:** Lab status is updated and credit is received after submission.
