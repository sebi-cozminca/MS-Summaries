---
title: 'TechLab: Understanding Microsoft Purview Insider Risk Management'
layout: default
nav_order: 84
parent: 'Lab summaries'
---

**ID** 168133  
**Number:** 41-411-5  
**Name:** TechLab: Understanding Microsoft Purview Insider Risk Management  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** True  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Enable permissions for insider risk management**
- **Goal:** Assign appropriate permissions for managing insider risk features in Microsoft Purview.
- **Actions:**
  - Sign in to the Purview portal as an admin.
  - Assign the "Insider Risk Management Admins" role group to the designated user (e.g., Joni Sherman).
  - Complete organizational setup if prompted.
- **Validation:**
  - Confirmation message for successful role assignment; user appears in the role group.

**Exercise 2: Confirm that the Microsoft 365 audit log has been enabled**
- **Goal:** Ensure audit logging is active to support insider risk management activities.
- **Actions:**
  - Navigate to the Audit section in the Purview portal.
  - Start recording user and admin activity if not already enabled.
- **Validation:**
  - Audit logging is enabled or in progress; confirmation or status message is visible.

**Exercise 3: Configure prerequisites for policies**
- **Goal:** Set up required integrations and policies for insider risk management.
- **Actions:**
  - Connect Microsoft 365 as a cloud app in Microsoft Defender.
  - Enable automatic scanning and file monitoring for Information Protection.
  - Create a Data Loss Prevention (DLP) policy with advanced rules (e.g., for IBAN detection and external sharing restrictions).
- **Validation:**
  - Cloud app is connected, file monitoring is enabled, and DLP policy is created and listed.

**Exercise 4: Create an insider risk management policy**
- **Goal:** Establish a policy to detect and manage insider risks based on DLP triggers.
- **Actions:**
  - Use the policy wizard to create a custom insider risk management policy (e.g., Data Leaks Test Policy).
  - Link the policy to the DLP Sample Policy and enable relevant risk indicators.
  - Review and submit the policy configuration.
- **Validation:**
  - Policy is created and appears in the policy list; confirmation message is displayed.

**Surveys**
- **Goal:** Collect user feedback before and after the lab.
- **Actions:**
  - Complete pre-lab and post-lab surveys.
- **Validation:**
  - Surveys submitted; lab completion is recorded.