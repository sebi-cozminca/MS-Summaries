---
title: 'Implement Insider Risk Management and Adaptive Protection - Ignite 2025'
layout: default
nav_order: 30
parent: 'Lab summaries'
---

**ID** 205051  
**Number:** LAB547  
**Name:** Implement Insider Risk Management and Adaptive Protection - Ignite 2025  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)  
**Additional licenses:** NA  
 
---

## Exercise Summary

**Exercise 1: Enable Analytics**
  - **Goal:** Activate analytics to surface organization-wide patterns of risky activity.
  - **Actions:**
    - Log into Microsoft Purview as an administrator.
    - Enable Insider Risk Management analytics at the tenant level and save settings.
  - **Validation:** Analytics are enabled and insights are available in the portal.

**Exercise 2: Configure Insider Risk Indicators**
  - **Goal:** Enable detection of risky AI and DLP activities.
  - **Actions:**
    - Enable indicators for risky prompts and responses in Copilot and other AI apps.
    - Add DLP policy alerts as indicators and select relevant policies.
    - Save the updated indicator settings.
  - **Validation:** Indicators for AI and DLP activities are active and visible in policy settings.

**Exercise 3: Create a Risky AI Usage Policy**
  - **Goal:** Detect and respond to risky AI usage for a specific project team.
  - **Actions:**
    - Create a custom policy using the Risky AI usage template.
    - Target the Mark 8 Project Team group and exclude Executives.
    - Prioritize SharePoint content, set activity triggers, and confirm indicator selection.
    - Apply built-in thresholds and submit the policy.
  - **Validation:** Policy is created and listed under Insider Risk Management policies.

**Exercise 4: Create a Notice Template**
  - **Goal:** Standardize user notifications for detected risky AI activity.
  - **Actions:**
    - Create a new notice template with a defined subject and HTML message body.
    - Save and verify the template in the portal.
  - **Validation:** Notice template appears in the list and is available for use in alerts.

**Exercise 5: Configure Insider Risk Levels**
  - **Goal:** Map AI usage policy to risk levels for adaptive enforcement.
  - **Actions:**
    - Assign the Risky AI usage policy to insider risk levels in Adaptive Protection settings.
    - Save the configuration.
  - **Validation:** Policy is linked to risk levels and reflected in Adaptive Protection.

**Exercise 6: Create a DLP Policy**
  - **Goal:** Block external sharing of sensitive data for users at elevated risk.
  - **Actions:**
    - Create a DLP policy using the U.S. PII Data Enhanced template.
    - Set the policy to apply when insider risk level is elevated.
    - Configure protection actions to block external sharing and run in simulation mode.
    - Enable policy tips and auto-activation after simulation.
  - **Validation:** DLP policy is created and visible in the Data Loss Prevention policies list.

**Exercise 7: Enable Adaptive Protection**
  - **Goal:** Automatically adjust DLP enforcement based on user risk level.
  - **Actions:**
    - Enable Adaptive Protection in the portal and save settings.
  - **Validation:** Adaptive Protection is active and DLP policies respond to risk level changes.

**Optional Exercise: Investigate Insider Risk Alerts with Security Copilot**
  - **Goal:** Explore alert investigation and triage using Security Copilot.
  - **Actions:**
    - Access the interactive demo to review and analyze insider risk alerts.
  - **Validation:** User can navigate the demo and understand alert investigation workflows.
