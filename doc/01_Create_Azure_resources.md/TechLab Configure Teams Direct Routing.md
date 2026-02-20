---
title: 'TechLab: Configure Teams Direct Routing'
layout: default
nav_order: 60
parent: 'Lab summaries'
---
 
**ID** 165887  
**Number:** 41-411-1  
**Name:** TechLab: Configure Teams Direct Routing  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** True  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise with Calling (Stakeholder: Kim Frank)  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Configuring the lab environment**
- **Goal:** Prepare the Microsoft Teams environment for Direct Routing by setting up DNS, Azure AD, and certificates.
- **Actions:**
  - Retrieve and register lab number and public IP with DNS delegation.
  - Add custom lab domain to Azure Active Directory and verify via TXT record.
  - Complete domain setup in Microsoft 365 admin center.
  - Request and obtain a public certificate for the SBC from DigiCert.
- **Validation:**
  - Domain appears as healthy in Microsoft 365 admin center; certificate is received and ready for use.

**Exercise 2: Configuring the session border controller**
- **Goal:** Assign custom domain to users and configure the AudioCodes SBC for Teams Direct Routing.
- **Actions:**
  - Assign custom lab domain to Teams users (Diego Siciliani, Patti Fernandez).
  - Download, import, and export public certificate to PFX format.
  - Upload SBC configuration and root certificates to the AudioCodes device.
  - Import lab certificate to SBC and update outbound manipulation set.
- **Validation:**
  - SBC configuration and certificates are successfully loaded; users have updated domain assignments.

**Exercise 3: Deploying Direct Routing in Microsoft 365**
- **Goal:** Connect the on-premises SBC to Microsoft Teams and enable/test Direct Routing for users.
- **Actions:**
  - Verify DNS records and test SBC connectivity via PowerShell and telnet.
  - Register SBC as an Online PSTN Gateway in Teams using PowerShell.
  - Validate SBC pairing in Teams admin center.
  - Enable debug logging and review SIP flows in Syslog Viewer.
  - Create PSTN usage and voice route; verify in Teams admin center.
  - Assign phone numbers and Direct Routing to users; confirm Teams Phone is enabled.
  - Create and assign voice routing policy to users.
  - Test inbound and outbound calls between Teams and 3CX softphone.
  - Review call records in SBC CDR History and Syslog Viewer.
- **Validation:**
  - Successful call connectivity between Teams and softphone; Teams admin center and Syslog Viewer confirm SBC status and call routing.
