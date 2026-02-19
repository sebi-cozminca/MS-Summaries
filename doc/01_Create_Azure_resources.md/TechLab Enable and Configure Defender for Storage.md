---
title: 'TechLab: Enable and Configure Defender for Storage'
layout: default
nav_order: 66
parent: 'Lab summaries'
---

**ID** 174317
**Number:** 41-411-4
**Name:** TechLab: Enable and Configure Defender for Storage
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Prepare the environment for Defender for Storage**
- **Goal:** Enable Microsoft Defender for Storage and set up the required Azure resources and local exclusions.
- **Actions:**
  - Enable Defender for Storage plan and upgrade the subscription in Azure.
  - Verify Defender for Storage and malware scanning settings are enabled.
  - Create a new storage account in Azure.
  - Exclude a local folder from Windows Security scanning.
- **Validation:**
  - Defender for Storage and malware scanning show as enabled in Azure.
  - Storage account is created and visible in the portal.
  - Folder exclusion is confirmed in Windows Security.

**Exercise 2: Test Defender for Storage**
- **Goal:** Validate Defender for Storage by uploading a test malware file and reviewing security alerts.
- **Actions:**
  - Create an EICAR test file and upload it to the storage account container.
  - Verify Defender for Cloud is enabled on the storage account.
  - Review blob scan results and Defender for Cloud security alerts for malicious file detection.
- **Validation:**
  - Blob index tag shows malware scan result as "Malicious."
  - High severity security alert appears in Defender for Cloud.

**Exercise 3: Configure automation to delete malicious files**
- **Goal:** Automate the deletion of malicious files detected by Defender for Storage.
- **Actions:**
  - Deploy a Logic App ARM template for blob deletion.
  - Assign Storage Blob Data Owner role to the Logic App and lab admin.
  - Change container authentication to Microsoft Entra user account.
  - Create workflow automation in Defender for Cloud to trigger the Logic App on malware alerts.
  - Upload a test malware file and observe automated deletion.
- **Validation:**
  - Malicious file is automatically deleted from the container.
  - Container shows "No blobs found" after automation runs.

**Exercise 4: Configure Log Analytics**
- **Goal:** Integrate Defender for Storage with Log Analytics for advanced monitoring and reporting.
- **Actions:**
  - Create a Log Analytics workspace in Azure.
  - Edit Defender for Cloud settings to send scan results to Log Analytics.
  - Disable workflow automation to allow file retention for analysis.
  - Upload a malware file and review scan results in Log Analytics using Kusto queries.
- **Validation:**
  - Log Analytics workspace receives and displays malware scan results for uploaded files.

**Exercise 5: Implement Azure Based Access Control (ABAC)**
- **Goal:** Restrict blob read access to only non-malicious files using ABAC conditions.
- **Actions:**
  - Remove previous role assignments and disable Logic App.
  - Assign Storage Blob Data Contributor role with a condition to allow read access only if "Malware scanning scan result" equals "No threats found."
  - Configure storage account to require Microsoft Entra authorization and disable key access.
  - Test access by uploading a malicious file and verifying access is denied.
- **Validation:**
  - Access to malicious blobs is denied as per ABAC condition.
  - Portal displays authorization error when attempting to read a malicious file.
