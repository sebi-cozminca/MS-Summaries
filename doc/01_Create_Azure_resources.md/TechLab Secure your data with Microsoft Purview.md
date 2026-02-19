---
title: 'TechLab: Secure your data with Microsoft Purview'
layout: default
nav_order: 79
parent: 'Lab summaries'
---

**ID** 185893
**Number:** 41-503-02
**Name:** TechLab: Secure your data with Microsoft Purview
**CloudSubscriptionPoolName:** NA
**AllowSave:** False
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

# TechLab Secure your data with Microsoft Purview — Exercise Summary

## Exercise Summary

**Exercise 1: Prepare your environment for compliance administration**
- **Goal:** Configure Microsoft Purview and onboard devices for compliance and data loss prevention.
- **Actions:**
  - Enable audit logging in Microsoft Purview.
  - Enable device onboarding and onboard a Windows device for endpoint DLP.
- **Validation:**
  - Audit logging and device onboarding are confirmed active in the portal; device is ready for DLP policies.

**Exercise 2: Create custom sensitive information types**
- **Goal:** Create a custom sensitive information type to detect and protect employee IDs.
- **Actions:**
  - Configure a new sensitive info type using regex and keyword lists in Microsoft Purview.
- **Validation:**
  - Custom sensitive info type appears in the portal and is available for use in policies.

**Exercise 3: Create sensitivity labels**
- **Goal:** Protect HR data by creating and publishing sensitivity labels for secure document handling.
- **Actions:**
  - Enable co-authoring for files with sensitivity labels.
  - Create a sensitivity label group and a label for HR employee data with dynamic watermarking.
  - Publish the sensitivity label for organization-wide use.
- **Validation:**
  - Sensitivity labels are visible and can be applied to HR documents; label policy is published.

**Exercise 4: Explore Data Security Posture Management (DSPM) for AI**
- **Goal:** Apply DSPM for AI recommendations to secure data and ensure compliance in AI interactions.
- **Actions:**
  - Review and apply DSPM for AI recommendations and policies in Microsoft Purview.
- **Validation:**
  - DSPM policies are created and visible in the portal; recommendations are applied.

**Exercise 5: Create a DLP policy**
- **Goal:** Implement and test a DLP policy to block sharing of sensitive data with generative AI platforms.
- **Actions:**
  - Create an endpoint DLP policy in simulation mode targeting generative AI websites.
  - (Optional) Activate the policy for enforcement.
- **Validation:**
  - DLP policy is created, tested, and optionally activated; policy status is visible in the portal.

**Exercise 6: Create an Insider Risk Management policy**
- **Goal:** Detect and address risky browsing behaviors that may expose sensitive data.
- **Actions:**
  - Configure insider risk settings and indicators.
  - Create a custom insider risk policy for risky browser usage.
- **Validation:**
  - Policy is created and configured; alerts are generated for risky activities.

**Exercise 7: Create an Adaptive Protection policy**
- **Goal:** Dynamically adjust DLP enforcement based on user risk levels using Adaptive Protection.
- **Actions:**
  - Enable Adaptive Protection in Insider Risk Management and link to the risk policy.
- **Validation:**
  - Adaptive Protection is enabled and configured; DLP policies adjust based on user risk.

**Lab Completion**
- **Validation:**
  - Submit the lab in the Skillable platform and confirm completion status in Viva and Learning Path the following week.
