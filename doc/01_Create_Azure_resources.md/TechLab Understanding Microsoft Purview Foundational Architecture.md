---
title: 'TechLab: Understanding Microsoft Purview Foundational Architecture'
layout: default
nav_order: 83
parent: 'Lab summaries'
---

**ID** 168136  
**Number:** 41-411-5  
**Name:** TechLab: Understanding Microsoft Purview Foundational Architecture  
**CloudSubscriptionPoolName:** NA  
**AllowSave:** True  
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise Blank 15S (Stakeholder: Kim Frank)  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Manage Compliance Roles**
- **Goal:** Assign compliance roles and enable auditing in Microsoft Purview.
- **Actions:**
  - Assign Compliance Admin role to a user following least privilege principles.
  - Enable auditing in the Purview portal and explore Activity Explorer.
  - Sign in as the assigned user to verify access and explore portal settings.
- **Validation:**
  - Confirmation of role assignment and ability to access compliance features as the assigned user.

**Exercise 2: Data Classification Basics**
- **Goal:** Understand and implement taxonomy and data classification in Microsoft Purview.
- **Actions:**
  - Learn taxonomy concepts and classification levels.
  - Review how to create and organize label taxonomies in Purview.
  - Explore classification and labeling features.
- **Validation:**
  - Knowledge check and review of taxonomy and classification setup.

**Exercise 3: Manage Sensitive Information Types**
- **Goal:** Create and test custom sensitive information types for data protection.
- **Actions:**
  - Create a custom sensitive info type for employee IDs using regex and keywords.
  - Build a keyword dictionary for disease-related terms and supporting keywords.
  - Test custom types by uploading sample files and verifying detection.
- **Validation:**
  - Successful detection of patterns in test files using the custom sensitive info types.

**Exercise 4: Manage Sensitivity Labels**
- **Goal:** Create, organize, and publish sensitivity labels for HR data.
- **Actions:**
  - Create a sensitivity label group and an HR-specific label with encryption settings.
  - Publish the labels and configure policy settings for HR users.
- **Validation:**
  - Labels are available for use and policy is published successfully.

**Exercise 5: Using Labels with the Microsoft Purview Information Protection Client (MPIP)**
- **Goal:** Apply sensitivity labels to files using the MPIP client.
- **Actions:**
  - Download and install the MPIP client.
  - Apply a sensitivity label to a file and verify encryption.
- **Validation:**
  - File displays a lock icon, indicating encryption is applied.

**Exercise 6: Encryption with Labeling**
- **Goal:** Apply and verify encryption on documents using sensitivity labels in Word.
- **Actions:**
  - Create and label Word documents with different sensitivity levels.
  - Test access restrictions by signing in as different users.
  - Attempt to open encrypted files in WordPad to verify encryption.
- **Validation:**
  - Access is restricted as configured; encrypted files cannot be opened in WordPad.

**Exercise 7: Auto-labeling**
- **Goal:** Configure auto-labeling policies for sensitive data.
- **Actions:**
  - Create an auto-labeling policy to apply labels to content containing U.S. Social Security Numbers.
- **Validation:**
  - Policy creation is confirmed (note: replication delay may prevent immediate validation).

**Exercise 8: Using Encryption with Office 365**
- **Goal:** Enable and verify email encryption using Purview.
- **Actions:**
  - Send an encrypted email from Outlook using the Encrypt option.
  - Open the email in an external account and verify encryption and access controls.
- **Validation:**
  - Recipient must use a one-time passcode or see protected message confirmation.

**Exercise 9: Data Security for Microsoft 365 with Copilot**
- **Goal:** Restrict data extraction rights to enhance security and compliance.
- **Actions:**
  - Edit a sensitivity label to remove copy/extract permissions, preventing Copilot from extracting data.
- **Validation:**
  - Label settings updated; extraction rights are removed.

**Exercise 10: Checking Actions with Activity Explorer**
- **Goal:** Monitor and analyze data activities using Activity Explorer.
- **Actions:**
  - Access Activity Explorer in the Purview portal to review data activity logs.
- **Validation:**
  - Activity Explorer is accessible (note: data population may be delayed due to audit log replication).

**Surveys**
- **Goal:** Collect user feedback before and after the lab.
- **Actions:**
  - Complete pre-lab and post-lab surveys.
- **Validation:**
  - Surveys submitted; lab completion is recorded.