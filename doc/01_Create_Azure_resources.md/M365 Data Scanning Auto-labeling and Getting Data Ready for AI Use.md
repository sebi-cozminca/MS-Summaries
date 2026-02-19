---
title: 'M365 Data Scanning, Auto-labeling and Getting Data Ready for AI Use'
layout: default
nav_order: 34
parent: 'Lab summaries'
---

**ID** 208642
**Number:** LAB 439
**Name:** M365 Data Scanning, Auto-labeling and Getting Data Ready for AI Use
**CloudSubscriptionPoolName:** NA
**AllowSave:** True
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Enable Audit in Microsoft Purview**
- **Goal:** Activate audit logging to track user and admin activity for compliance and labeling features.
- **Actions:**
  - Log into the Microsoft Purview portal as Megan Bowen.
  - Navigate to Solutions > Audit and enable audit logging.
- **Validation:**
  - Audit logging is enabled; the blue notification bar disappears.

**Exercise 2: Create a Custom Sensitive Information Type (SIT)**
- **Goal:** Define a custom SIT to detect Contoso project codes for targeted data protection.
- **Actions:**
  - Navigate to Information Protection > Sensitive info types.
  - Create a new SIT with a regex pattern and supporting keywords for project codes.
- **Validation:**
  - Custom SIT "Contoso Project Codes" is created and visible in the portal.

**Exercise 3: Test Custom Sensitive Information Types**
- **Goal:** Validate that the custom SIT correctly detects project codes in sample content.
- **Actions:**
  - Create a test file with a sample project code.
  - Upload and test the file in the Purview portal using the SIT test feature.
- **Validation:**
  - SIT test results confirm correct detection of project codes.

**Exercise 4: Create a Sensitivity Label Group**
- **Goal:** Organize sensitivity labels for internal and project-specific data.
- **Actions:**
  - Enable sensitivity labels for SharePoint and OneDrive.
  - Create a label group named "Internal" with appropriate descriptions.
- **Validation:**
  - Label group "Internal" is created and available for label organization.

**Exercise 5: Create a Label in the Group for Project Data**
- **Goal:** Define a sensitivity label for project data to support auto-labeling and protection.
- **Actions:**
  - Create a "Project data" label in the Internal group with content marking (footer).
  - Configure scope for files and emails.
- **Validation:**
  - Project data label is created and applies a visible footer to labeled content.

**Exercise 6: Publish Sensitivity Labels**
- **Goal:** Make sensitivity labels available for manual and automated application across workloads.
- **Actions:**
  - Publish the Internal/Project data label using a label publishing policy.
- **Validation:**
  - Labels are published and available for use in policies and by users.

**Exercise 7: Configure Auto-Apply Labeling**
- **Goal:** Automatically classify content containing project codes with the Project data label.
- **Actions:**
  - Create an auto-labeling policy targeting the custom SIT.
  - Set up rules to apply the Project data label in Exchange, SharePoint, and OneDrive.
- **Validation:**
  - Policy is created and runs in simulation mode; content with project codes is auto-labeled.

**Exercise 8: Configure Default Sensitivity Labels**
- **Goal:** Enforce a baseline protection level by applying default labels to new content.
- **Actions:**
  - Create a default labeling policy for documents, emails, meetings, and Power BI content.
  - Set "General/All Employees (unrestricted)" as the default label.
- **Validation:**
  - Default label is automatically applied to new content across supported workloads.

**Bonus Exercise: Create a DLP Policy in Simulation Mode**
- **Goal:** Prevent Microsoft 365 Copilot from processing content labeled as project data.
- **Actions:**
  - Create a DLP policy in Microsoft Purview targeting the Project data label.
  - Configure the policy to restrict Copilot processing and run in simulation mode.
- **Validation:**
  - DLP policy is active in simulation mode; Copilot is restricted from processing labeled content.