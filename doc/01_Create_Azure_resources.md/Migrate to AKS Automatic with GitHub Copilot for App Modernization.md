---
title: 'Migrate to AKS Automatic with GitHub Copilot for App Modernization'
layout: default
nav_order: 37
parent: 'Lab summaries'
---

**ID** 205052
**Number:** LAB 110
**Name:** Migrate to AKS Automatic with GitHub Copilot for App Modernization
**CloudSubscriptionPoolName:** Microsoft TechConnect 2026-PRODMCA-CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** Events GHE w/ Copilot

---

# Migrate to AKS Automatic with GitHub Copilot for App Modernization - Lab Instruction Summary

## Exercise Summary

**Exercise 1: Environment Setup and Prerequisites**
- **Goal:** Prepare the local and cloud environment for application modernization and migration.
- **Actions:**
  - Sign in to Azure and configure Azure CLI.
  - Install the Azure Service Connector extension and create a service connector for PostgreSQL Flexible Server.
  - Configure Azure RBAC authentication for kubectl and obtain AKS credentials.
  - Authenticate GitHub Copilot and VS Code with provided accounts.
- **Validation:**
  - Successful Azure login, service connector creation, kubectl access to AKS, and Copilot authentication.

**Exercise 2: Verify and Explore PetClinic Locally**
- **Goal:** Confirm the Spring Boot PetClinic app runs locally with PostgreSQL and explore its features.
- **Actions:**
  - Start the PetClinic app with Maven and connect to local PostgreSQL.
  - Access the app in a browser and test core features (owners, pets, veterinarians).
- **Validation:**
  - Application accessible at http://localhost:8080 and all features function as expected.

**Exercise 3: Application Modernization with GitHub Copilot**
- **Goal:** Assess and modernize the PetClinic app for cloud readiness using GitHub Copilot App Modernization.
- **Actions:**
  - Run the assessment tool to analyze the codebase for migration issues and modernization opportunities.
  - Review assessment results and focus on database migration to Azure PostgreSQL Flexible Server with Entra ID authentication.
  - Select and execute the guided migration task for PostgreSQL (Spring option).
  - Review and approve migration plan and progress in generated markdown files.
- **Validation:**
  - Migration plan and progress files confirm successful code and configuration updates for managed identity authentication.

**Exercise 4: Validation and Automated Fixes**
- **Goal:** Ensure the modernized application is secure, functional, and consistent post-migration.
- **Actions:**
  - Allow the tool to run validation stages: CVE scanning, build validation, consistency checks, and test execution.
  - Review and approve or manually fix issues as needed.
- **Validation:**
  - All validation stages pass; application builds and tests succeed with managed identity authentication.

**Exercise 5: Generate Containerization Assets with AI**
- **Goal:** Create Docker and Kubernetes manifests for the modernized application using AI-powered tools.
- **Actions:**
  - Use Copilot agent chat to generate Dockerfile and Kubernetes manifests (Deployment, Service) with workload identity and secret integration.
  - Review and tune generated manifests for environment-specific settings.
- **Validation:**
  - Containerization assets are created in the k8s/ directory and ready for deployment.

**Exercise 6: Build and Push Container Image to ACR**
- **Goal:** Build and store the application container image in Azure Container Registry.
- **Actions:**
  - Log in to ACR and build the Docker image using Azure CLI.
- **Validation:**
  - Image is successfully built and available in ACR.

**Exercise 7: Deploy to AKS Automatic**
- **Goal:** Deploy the modernized, containerized application to AKS Automatic with secure database connectivity.
- **Actions:**
  - Apply Kubernetes manifests to deploy the app to AKS.
  - Monitor deployment status and verify pod readiness.
  - Port-forward to access the app and test Entra ID authentication.
  - Check pod environment variables and logs for passwordless authentication.
- **Validation:**
  - Application is accessible via AKS, uses managed identity for PostgreSQL, and passes all connectivity and authentication checks.

**Exercise 8: Troubleshooting and Validation**
- **Goal:** Resolve common deployment and connectivity issues and validate production readiness.
- **Actions:**
  - Use provided troubleshooting steps for Docker, PostgreSQL, and AKS Service Connector.
  - Retrieve and verify Service Connector YAML configuration and secret references.
  - Compare deployment file with provided example for correctness.
- **Validation:**
  - Application and database connectivity issues are resolved; deployment file matches best practices for AKS Automatic.
