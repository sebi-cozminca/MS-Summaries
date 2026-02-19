---
title: 'TechLab: Enable and Configure Defender for Cloud'
layout: default
nav_order: 65
parent: 'Lab summaries'
---

**ID** 173542
**Number:** 41-411-4
**Name:** TechLab: Enable and Configure Defender for Cloud
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)
**AllowSave:** True
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Enable Microsoft Defender for Cloud**
- **Goal:** Enable and configure Microsoft Defender for Cloud on an Azure subscription and import lab resources.
- **Actions:**
  - Sign in to Azure portal and access Microsoft Defender for Cloud.
  - Enable and upgrade Defender plans for the subscription.
  - Import sample resources via custom ARM template deployment, editing template parameters as required.
- **Validation:**
  - Defender plans show as enabled for the subscription.
  - Resource deployment completes successfully and resources are visible in Azure.

**Exercise 2: Understand the Microsoft Defender for Cloud Dashboard**
- **Goal:** Explore the main dashboards and pages of Microsoft Defender for Cloud.
- **Actions:**
  - Review the Overview, Azure subscriptions, Security posture, Regulatory compliance, Workload protections, Inventory, Firewall Manager, Data security, Cloud Security Explorer, and DevOps security pages.
  - Observe available security insights, compliance controls, and resource coverage.
- **Validation:**
  - All dashboard pages are accessible and display relevant security and compliance information.

**Exercise 3: Explore Secure Score and Recommendations**
- **Goal:** Assess Secure Score and review security recommendations in Defender for Cloud.
- **Actions:**
  - Review Secure Score and environment risks on the Security posture page.
  - Explore security controls and download recommendations reports.
  - Investigate specific recommendations, review remediation options, and apply quick fixes.
- **Validation:**
  - Secure Score and recommendations are visible.
  - Remediation actions complete and notifications confirm success.

**Exercise 4: Explore Inventory Capabilities**
- **Goal:** Utilize the Asset Inventory dashboard to analyze and filter resources covered by Defender for Cloud.
- **Actions:**
  - Review total and unhealthy resources in Inventory.
  - Use search and filters to locate specific resources and recommendations.
  - Open Azure Resource Graph Explorer to run and save inventory queries.
- **Validation:**
  - Inventory reflects correct resource counts and filter results.
  - Queries return expected resource data.

**Exercise 5: Overview of Microsoft Defender for Cloud Policies**
- **Goal:** Review, edit, and enforce security policies and exemptions in Defender for Cloud.
- **Actions:**
  - Review security policies and standards assigned to the subscription.
  - Explore Azure Policy definitions and initiatives related to security.
  - Create resource exemptions for recommendations and set expiration and waiver details.
  - Enforce policies by applying Deny and Enforce actions on recommendations.
- **Validation:**
  - Policy changes and exemptions are reflected in Azure Policy and Defender for Cloud.
  - Enforcement actions are applied and visible in the portal.
