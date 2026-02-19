---
title: 'Prevent data exposure in Copilot and AI apps with Data Loss Prevention - Ignite 2025'
layout: default
nav_order: 43
parent: 'Lab summaries'
---

**ID** 205170
**Number:** LAB548
**Name:** Prevent data exposure in Copilot and AI apps with Data Loss Prevention - Ignite 2025
**CloudSubscriptionPoolName:** NA
**AllowSave:** False
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Create a DLP Policy in Simulation Mode**
- **Goal:** Restrict Microsoft 365 Copilot from processing highly confidential content using a DLP policy in simulation mode.
- **Actions:**
  - Access Microsoft Purview portal and navigate to Data Loss Prevention policies.
  - Create a custom DLP policy targeting Microsoft 365 Copilot and Copilot Chat for the "Mark 8 Project Team" group.
  - Add a rule to restrict Copilot from processing content labeled as Highly Confidential.
  - Set the policy to run in simulation mode with policy tips enabled.
- **Validation:**
  - Policy appears in simulation mode and restricts Copilot access to specified content.

**Exercise 2: Activate a Policy in Simulation Mode**
- **Goal:** Move the Copilot DLP policy from simulation to active enforcement and review simulation insights.
- **Actions:**
  - Review simulation overview, items for review, and alerts in the policy's simulation view.
  - Activate the policy by turning it on and confirming publication.
- **Validation:**
  - Policy status changes to active and enforcement is enabled.

**Exercise 3: Create an Endpoint DLP Policy**
- **Goal:** Block users from pasting or uploading banking data into AI websites using endpoint DLP.
- **Actions:**
  - Create a custom endpoint DLP policy for devices in Microsoft Purview.
  - Add rules to detect sensitive info types (credit card, routing numbers, etc.).
  - Configure actions to block uploads and pastes to generative AI websites, with user notifications.
  - Set policy to turn on immediately.
- **Validation:**
  - Policy is created and blocks banking data exposure to AI websites as configured.

**Exercise 4: Configure DLP Alert Settings**
- **Goal:** Route DLP incident alerts to the appropriate administrator with correct severity.
- **Actions:**
  - Edit the endpoint DLP policy rule to set alert severity to Medium.
  - Enable admin alerts and add MOD Administrator as recipient.
  - Set alerts to trigger on every rule match.
- **Validation:**
  - Alerts are sent to the MOD Administrator for each incident with correct severity.

**Exercise 5: Configure DLP Alert Aggregation**
- **Goal:** Aggregate multiple DLP alerts from the same user within a set time window.
- **Actions:**
  - Enable alert aggregation by user in DLP settings.
  - Set aggregation window to 30 minutes and save settings.
- **Validation:**
  - Multiple DLP detections from the same user within 30 minutes are combined into a single alert.

**Bonus Exercise: Implement Adaptive Protection**
- **Goal:** Dynamically enforce DLP policies based on insider risk signals using Adaptive Protection.
- **Actions:**
  - Edit the endpoint DLP rule to apply only to users with elevated insider risk.
  - Create a quick policy for risky AI usage in Insider Risk Management.
  - Link the risky AI usage policy to Adaptive Protection and enable it for DLP.
- **Validation:**
  - DLP enforcement is dynamically applied only to users flagged as elevated risk, reducing friction for others.
