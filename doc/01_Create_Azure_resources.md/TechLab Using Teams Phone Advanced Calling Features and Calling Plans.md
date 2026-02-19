---
title: 'TechLab: Using Teams Phone Advanced Calling Features and Calling Plans'
layout: default
nav_order: 87
parent: 'Lab summaries'
---

**ID** 165886
**Number:** 41-411-1
**Name:** TechLab: Using Teams Phone Advanced Calling Features and Calling Plans
**CloudSubscriptionPoolName:** NA
**AllowSave:** True
**CloudCredentialPoolAssignments:** WWL | M365 Enterprise with Calling (Stakeholder: Kim Frank)
**Additional licenses:** NA

---

# Exercise Summary

**Exercise 1: Configuring global Teams settings and user policies**
- **Goal:** Set up Teams calling and voicemail policies for compliance and regional requirements.
- **Actions:**
  - Enable cloud recording for calling in the global policy.
  - Create and assign a custom calling policy for recording, transcription, and busy-on-busy.
  - Create a voicemail policy for Germany with language, profanity mask, and transcription settings.
- **Validation:**
  - Policies are created, assigned, and reflected in Teams admin center.

**Exercise 2: Streamlining administration with PowerShell**
- **Goal:** Use PowerShell to manage Teams voicemail policies and group assignments.
- **Actions:**
  - Retrieve and verify voicemail policies.
  - Create a marketing group and assign members.
  - Assign voicemail policies to group members and verify assignments in Teams admin center.
- **Validation:**
  - Group and policy assignments are visible in Teams admin center and PowerShell output.

**Exercise 3: Configure Calling Plans**
- **Goal:** Enable and assign Teams Calling Plan licenses, phone numbers, and emergency locations.
- **Actions:**
  - Assign Domestic Calling Plan licenses to users.
  - Add emergency locations and order phone numbers.
  - Assign phone numbers to users and configure call forwarding.
- **Validation:**
  - Users have assigned licenses and phone numbers; call settings are updated in Teams admin center.

**Exercise 4: Configure and license resource accounts for Auto Attendants and Call Queues**
- **Goal:** Set up resource accounts, license them, and assign phone numbers for auto attendants and call queues.
- **Actions:**
  - Create and license resource accounts for auto attendant and call queue.
  - Order and assign phone numbers to resource accounts.
- **Validation:**
  - Resource accounts are licensed and have assigned phone numbers in Teams admin center.

**Exercise 5: Create a call queue, auto attendant, and voice applications policy**
- **Goal:** Deploy and configure call queues, auto attendants, and related voice policies.
- **Actions:**
  - Configure holidays and after-hours call flows.
  - Create and configure a call queue and auto attendant with menu options.
  - Create and assign a custom voice applications policy.
- **Validation:**
  - Call queue and auto attendant are operational; policies are assigned and visible in Teams admin center.

**Exercise 6: Working with voice features**
- **Goal:** Implement advanced voice features and policies for Teams Phone.
- **Actions:**
  - Add caller ID, emergency, and call park policies.
  - Configure after-hours and holiday call flows, dial plans, and shared line appearance.
  - Set up routing rules for unassigned numbers and test routing.
- **Validation:**
  - Policies and routing rules are active; test calls and settings reflect changes.

**Exercise 7: Using voice enabled channels (Collaborative Calling)**
- **Goal:** Integrate call queues with Teams channels for collaborative calling.
- **Actions:**
  - Create a new channel for call queue integration.
  - Configure the call queue to use the channel and test call routing.
- **Validation:**
  - Calls to the queue are routed to the Teams channel; notifications and call handling work as expected.

**Exercise 8: Reviewing Operator Connect**
- **Goal:** Explore Operator Connect as a PSTN connectivity option for Teams.
- **Actions:**
  - Review Operator Connect offers and operator details in Teams admin center.
- **Validation:**
  - Operator options and offer details are accessible and reviewed.

**Clean up**
- **Goal:** Release phone numbers and clean up lab resources.
- **Actions:**
  - Remove phone numbers from users and resource accounts using PowerShell.
  - Release numbers back to the service.
- **Validation:**
  - Phone numbers are unassigned and released; tenant resources are cleaned up.