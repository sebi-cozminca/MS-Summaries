---
title: 'Govern identities with confidence using Microsoft Entra - Ignite 2025'
layout: default
nav_order: 28
parent: 'Lab summaries'
---

**ID** 205271  
**Number:** LAB544  
**Name:** Govern identities with confidence using Microsoft Entra - Ignite 2025  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)  
**Additional licenses:** M365Copilot  

---

## Exercise Summary

**Exercise 1: Add an ID Governance Trial License**
  - **Goal:** Enable Microsoft Entra ID Governance features by activating a trial license.
  - **Actions:**
    - Log into the lab environment and Entra admin center with provided credentials.
    - Navigate to Billing > Trials and activate the Microsoft Entra ID Governance trial.
  - **Validation:** Trial license is activated and visible in the admin center.

**Exercise 2: Build a Catalog in Microsoft Entra Entitlement Management**
  - **Goal:** Set up a resource catalog and access package for streamlined access management.
  - **Actions:**
    - Create a new catalog (catSales) and add groups, applications, SharePoint sites, and Entra roles as resources.
    - Create an access package (pkgSales) linked to the catalog, configure resource roles, and set assignment and lifecycle policies.
  - **Validation:** Catalog and access package are created; resources and roles are correctly assigned and visible in the portal.

**Exercise 3: Onboard a New Hire with Lifecycle Workflows**
  - **Goal:** Automate onboarding for new users using Lifecycle workflows.
  - **Actions:**
    - Create a joiner workflow triggered by department attribute change.
    - Configure tasks to enable account, send welcome email, add to group, assign access package, and assign licenses.
    - Enable and schedule the workflow.
  - **Validation:** Workflow is created, enabled, and visible in the Lifecycle workflows list; tasks are configured as required.

**Exercise 4: Add a New User and Test Workflow and Entitlement**
  - **Goal:** Validate onboarding and entitlement assignment for a new user.
  - **Actions:**
    - Create a new user with department set to trigger the workflow.
    - Manually run the workflow if needed and monitor task status.
    - Log in as the new user to confirm group, application, and role assignments.
    - Test just-in-time access activation for privileged roles.
    - Optionally, modify access package resources and reprocess assignments.
  - **Validation:** New user receives correct group, application, and role assignments; workflow tasks complete with status reporting.

**Exercise 5: Confirm Access with Access Reviews**
  - **Goal:** Ensure only authorized users retain access to sensitive applications using access reviews.
  - **Actions:**
    - Create a new access review for the LinkedIn application, configure reviewers, recurrence, and actions for non-response.
    - Monitor review status and confirm reviewer assignment.
    - (Lab limitation) Understand review process even if email notifications are not sent in the sandbox.
  - **Validation:** Access review is created, active, and assigned to the correct reviewer; review results and audit logs are visible in the portal.
