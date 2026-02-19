---
title: 'Defend against threats with Microsoft Defender XDR - Ignite 2025'
layout: default
nav_order: 21
parent: 'Lab summaries'
---

**ID** 205058
**Number:** LAB541
**Name:** Defend against threats with Microsoft Defender XDR - Ignite 2025
**CloudSubscriptionPoolName:** NA
**AllowSave:** False
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Explore Microsoft Defender XDR**
- **Goal:** Familiarize with Microsoft Defender XDR and configure preset security policies for Exchange Online Protection (EOP) and Microsoft Defender for Office 365.
- **Actions:**
  - Obtain Microsoft 365 tenant credentials from the lab provider.
  - Sign in to the Microsoft Defender XDR portal.
  - Apply preset security policies for EOP and Defender for Office 365 (Standard and Strict protection) to specific recipients and groups.
  - Prepare and initialize the Defender XDR workspace.
- **Validation:**
  - Policies are enabled and visible in the portal; workspace initialization completes with all features available.

**Exercise 2: Deploy Microsoft Defender for Endpoint**
- **Goal:** Deploy and configure Microsoft Defender for Endpoint, onboard devices, and set up security roles and device groups.
- **Actions:**
  - Initialize Microsoft Defender for Endpoint in the Defender XDR portal.
  - Onboard a device using the local onboarding script and confirm successful onboarding.
  - Configure custom security roles (e.g., Tier 1 Support) with appropriate permissions and assignments.
  - Create and configure device groups with remediation levels and user access.
- **Validation:**
  - Device appears as onboarded in the portal; roles and device groups are listed and applied as configured.

**Exercise 3: Mitigate Attacks with Microsoft Defender for Endpoint**
- **Goal:** Test Defender for Endpoint's detection and response by simulating attacks and investigating alerts/incidents.
- **Actions:**
  - Verify device onboarding and run a detection test script to generate alerts.
  - Investigate generated alerts and incidents in the Defender XDR portal, reviewing alert details, recommendations, and incident timelines.
  - Simulate an attack using a provided PowerShell script and observe Defender's response.
  - Investigate the simulated attack as a single incident, review the incident graph, and analyze evidence and response details.
- **Validation:**
  - Alerts and incidents are generated and visible in the portal; investigation steps confirm Defender's detection and response capabilities.
