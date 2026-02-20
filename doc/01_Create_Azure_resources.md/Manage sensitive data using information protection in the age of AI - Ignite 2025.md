---
title: 'Manage sensitive data using information protection in the age of AI - Ignite 2025'
layout: default
nav_order: 37
parent: 'Lab summaries'
---

**ID** 205050  
**Number:** LAB545  
**Name:** Manage sensitive data using information protection in the age of AI - Ignite 2025  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** True  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Enable Audit in Microsoft Purview Portal**
- **Goal:** Activate audit logging to track user and admin activity for compliance and labeling features.
- **Actions:**
  - Log in to Microsoft Purview as Megan Bowen.
  - Navigate to Audit under Solutions and enable audit logging.
- **Validation:**
  - Blue bar disappears, confirming audit is enabled.

**Exercise 2: Create a Custom Sensitive Information Type (SIT)**
- **Goal:** Define a custom SIT to detect Contoso project codes for targeted protection.
- **Actions:**
  - Access Information Protection > Sensitive info types.
  - Create a new SIT with a regex pattern and supporting keyword list for project codes.
- **Validation:**
  - SIT appears in the list and is available for use in policies.

**Exercise 3: Test Custom Sensitive Information Types**
- **Goal:** Validate that the custom SIT correctly detects project codes in content.
- **Actions:**
  - Create a test file with a sample project code.
  - Upload and test the file in the Purview portal using the SIT's Test feature.
- **Validation:**
  - Match results confirm the SIT detects the project code as expected.

**Exercise 4: Create a Sensitivity Label Group**
- **Goal:** Organize sensitivity labels for internal and project-specific data.
- **Actions:**
  - Enable support for sensitivity labels in SharePoint/OneDrive.
  - Create a label group named Internal with appropriate descriptions.
- **Validation:**
  - Label group appears in the Sensitivity labels section.

**Exercise 5: Create a Label in the Group for Project Data**
- **Goal:** Define a sensitivity label for project data to support auto-labeling and content marking.
- **Actions:**
  - Add a new label under the Internal group for project data.
  - Configure scope, content marking (footer), and descriptions.
- **Validation:**
  - Label is created and available for publishing.

**Exercise 6: Publish Sensitivity Labels**
- **Goal:** Make the new sensitivity label available for manual and automated use.
- **Actions:**
  - Publish the Internal/Project data label via a label publishing policy.
  - Name and submit the policy for deployment.
- **Validation:**
  - Label is available for selection in policies and user interfaces.

**Exercise 7: Configure Auto-Apply Labeling**
- **Goal:** Automatically apply the Project data label to content containing project codes.
- **Actions:**
  - Create an auto-labeling policy targeting Exchange, SharePoint, and OneDrive.
  - Define a rule using the custom SIT to trigger labeling.
  - Set policy to simulation mode for initial rollout.
- **Validation:**
  - Policy is created and will auto-label matching content in simulation mode.

**Exercise 8: Configure Default Sensitivity Labels**
- **Goal:** Enforce a baseline protection level by applying default labels to new content.
- **Actions:**
  - Create a label publishing policy to set General/All Employees (unrestricted) as the default for documents, emails, meetings, and Fabric content.
  - Require justification for label removal or lowering classification.
- **Validation:**
  - Default label is automatically applied to new content across supported workloads.

**Bonus Exercise: Create a DLP Policy in Simulation Mode**
- **Goal:** Prevent Microsoft 365 Copilot from processing content labeled as project data.
- **Actions:**
  - Create a DLP policy targeting Copilot and Copilot Chat locations.
  - Add a rule to restrict Copilot from accessing content with the Project data label.
  - Run the policy in simulation mode with policy tips enabled.
- **Validation:**
  - DLP policy is active in simulation mode, restricting Copilot's access to labeled content.
