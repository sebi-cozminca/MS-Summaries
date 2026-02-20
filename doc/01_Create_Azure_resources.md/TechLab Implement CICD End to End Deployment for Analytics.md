---
title: 'TechLab: Implement CI/CD End to End Deployment for Analytics'
layout: default
nav_order: 70
parent: 'Lab summaries'
---

**ID** 168512  
**Number:** 41-411-7  
**Name:** TechLab: Implement CI/CD End to End Deployment for Analytics  
**CloudSubscriptionPoolName:** CSU - DevOps Parallellism (UAT)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Understanding Key Concepts of CI/CD**
- **Goal:** Grasp the principles and benefits of CI/CD for analytics using Azure Data Factory and Databricks.
- **Actions:**
  - Review CI/CD concepts, lifecycle steps, and architecture diagrams for ADF and Databricks.
- **Validation:** Understanding of CI/CD concepts and their application in Azure analytics environments.

**Exercise 2: Set up CI for Azure Data Factory using Azure DevOps**
- **Goal:** Establish continuous integration for ADF pipelines with Azure DevOps.
- **Actions:**
  - Create Azure DevOps project and repository, configure reviewer policy.
  - Generate a Personal Access Token (PAT).
  - Configure ADF to use Azure Repos Git and set up collaboration/publish branches.
  - Create feature branch, develop/debug pipeline, configure source and sink with Azure Key Vault and Blob Storage.
  - Upload sample data, create pull request, review and merge changes, and publish main branch in ADF.
- **Validation:** Pipeline changes are merged, published, and source control integration is functional.

**Exercise 3: Set up CD for Azure Data Factory by using Azure DevOps**
- **Goal:** Implement continuous deployment for ADF pipelines.
- **Actions:**
  - Create Dev and Prod variable groups in Azure DevOps.
  - Build ARM template stage and configure deployment to Dev environment.
  - Enable continuous integration triggers and deploy to Dev.
  - Create release pipeline for Prod deployment and enable continuous deployment triggers.
- **Validation:** Successful deployment to Dev and Prod environments via Azure DevOps pipelines.

**Exercise 4: Validation/Deployment for ADF Prod**
- **Goal:** Validate and monitor production deployment of ADF pipelines.
- **Actions:**
  - Monitor deployment process in ADF and Azure DevOps.
  - Confirm pipeline and activity status, save and publish changes.
- **Validation:** Deployment completes successfully and pipelines are operational in production.

**Exercise 5: Continuous Integration configuration (Databricks)**
- **Goal:** Set up CI for Databricks notebooks and resources using Azure DevOps.
- **Actions:**
  - Create Azure DevOps project and initialize/clone Git repository.
  - Configure Databricks workspace, import and organize notebooks, commit changes to repo.
  - Generate Databricks access tokens and configure Data Factory integration.
  - Develop and deploy Databricks pipelines via ADF, test connections, and publish.
- **Validation:** Notebooks and pipelines are versioned, tested, and integrated with ADF and Azure DevOps.

**Exercise 6: Configure Azure DevOps pipelines for Databricks**
- **Goal:** Automate build and artifact publishing for Databricks resources.
- **Actions:**
  - Create build pipeline in Azure DevOps, add Publish Build Artifacts task.
  - Enable continuous integration triggers and run the pipeline.
- **Validation:** Build artifacts are published and pipeline runs successfully.

**Exercise 7: Deploy and manage releases for Databricks**
- **Goal:** Automate deployment of Databricks notebooks to Dev and Prod environments.
- **Actions:**
  - Create release pipeline, add Databricks Script Deployment Task, configure deployment parameters.
  - Enable continuous deployment triggers, create and monitor releases.
  - Retrieve and use production Databricks tokens and region info for Prod deployment.
- **Validation:** Notebooks are deployed to Databricks Dev and Prod workspaces; release status is successful.

**Exercise 8: Lab Completion**
- **Goal:** Complete the lab and provide feedback.
- **Actions:**
  - Answer survey questions and submit responses to mark lab as complete.
- **Validation:** Lab completion is recorded and feedback is submitted.
