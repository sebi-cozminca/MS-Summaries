---
title: 'Zero Trust Lab: Securing Identities and Devices with Intune & Entra - Ignite 2025'
layout: default
nav_order: 95
parent: 'Lab summaries'
---

**ID** 205066  
**Number:** LAB542  
**Name:** Zero Trust Lab: Securing Identities and Devices with Intune & Entra - Ignite 2025  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise 2019 w/ SPE_E (Stakeholder: Kim Frank)   
**Additional licenses:** NA  

---

## Exercise Summary

**Section 1: Install the Zero Trust Assessment Tool**
- **Goal:** Set up the Zero Trust Assessment module to evaluate tenant security posture.
- **Actions:**
  - Log in to the lab VM and access the Zero Trust Workshop site.
  - Install the ZeroTrustAssessment PowerShell module as administrator.
- **Validation:**
  - Module installs successfully and is ready for use.

**Section 2: Run and Review the Zero Trust Assessment**
- **Goal:** Assess and review the current Zero Trust security configuration.
- **Actions:**
  - Connect to Microsoft Graph using the assessment module with Global Admin credentials.
  - Run the assessment and generate a report.
  - Review the assessment report in Microsoft Edge, focusing on Identity and Devices tabs.
- **Validation:**
  - Assessment report is generated and accessible, showing configuration checks and recommendations.

**Section 3: Enforce Phishing-Resistant MFA for Privileged Roles**
- **Goal:** Protect privileged Entra roles by requiring phishing-resistant MFA.
- **Actions:**
  - Sign in to Entra admin center and create a Conditional Access policy.
  - Target privileged roles and require phishing-resistant MFA strength.
  - Set policy to Report-only mode for testing.
- **Validation:**
  - Policy is created and visible in Conditional Access, set to Report-only.

**Section 4: Block Legacy Authentication**
- **Goal:** Prevent use of insecure legacy authentication protocols.
- **Actions:**
  - Create a Conditional Access policy to block legacy authentication for all users.
  - Configure client app conditions and set policy to On.
- **Validation:**
  - Policy is active and blocks legacy authentication attempts.

**Section 5: Deploy a Windows LAPS Policy with Intune**
- **Goal:** Securely manage local admin passwords using Windows LAPS and Intune.
- **Actions:**
  - Create a Windows LAPS policy in Intune with specified complexity and backup settings.
  - Assign policy to devices and enable LAPS in Entra admin center.
- **Validation:**
  - LAPS policy is deployed and enabled for managed devices.

**Section 6: Create and Assign an Intune Compliance Policy**
- **Goal:** Define and enforce minimum security standards for Windows devices.
- **Actions:**
  - Create a compliance policy in Intune requiring BitLocker, Secure Boot, and Defender Antimalware.
  - Assign policy to all devices or a test group.
- **Validation:**
  - Compliance policy is active and devices are evaluated for compliance.

**Section 7: Require Device Compliance with Conditional Access**
- **Goal:** Restrict access to resources to only compliant or protected devices.
- **Actions:**
  - Use Conditional Access templates to require compliant or hybrid Azure AD joined devices or MFA for all users.
  - Review and create the policy in Report-only mode.
- **Validation:**
  - Policy is created and visible in Conditional Access, set to Report-only.

**Bonus Exercises: Review and Explore Zero Trust Tools**
- **Goal:** Deepen understanding of Zero Trust controls and available resources.
- **Actions:**
  - Review additional assessment items and remediation steps in the demo report.
  - Explore the Zero Trust Workshop tool and related Microsoft Learn documentation.
- **Validation:**
  - Additional controls and resources are reviewed and understood for future application.
