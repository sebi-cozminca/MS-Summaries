---
title: 'Connect, secure and manage hybrid, multicloud and edge with Azure Arc'
layout: default
nav_order: 18
parent: 'Lab summaries'
---

**ID** 205275
**Number:** LAB504
**Name:** Connect, secure and manage hybrid, multicloud and edge with Azure Arc
**CloudSubscriptionPoolName:** Microsoft Events 25 - MSLEARN CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Connect, Secure, and Manage Hybrid Multicloud and Edge with Azure Arc — Lab Instruction Summary

## Exercise Summary

**Module 1: Onboard a Windows VM**
- **Goal:** Register and onboard a Windows VM to Azure Arc for hybrid management.
- **Actions:**
  - Register the Microsoft.HybridCompute resource provider in Azure.
  - Use the Azure Arc Setup wizard to install the Azure Connected Machine agent and connect the VM to Azure.
  - Authenticate with Azure, select resource group and region, and complete onboarding.
  - Verify the VM appears in Azure Arc resources and review available management capabilities.
- **Validation:**
  - VM is listed as an Azure Arc-enabled machine in the portal; management features are accessible.

**Module 2: Enable Monitoring with Azure Monitor Agent**
- **Goal:** Enable monitoring and log collection for the Arc-enabled VM using Azure Monitor.
- **Actions:**
  - Create a Log Analytics workspace (ArcLogWorkspace) in East US.
  - Add the Azure Monitor Agent extension to the Arc-enabled VM.
  - Create a Data Collection Rule (DCR) for performance counters and Windows event logs, targeting the Log Analytics workspace.
  - Verify data ingestion by running KQL queries for performance and event logs in the workspace.
- **Validation:**
  - Performance and event log data from the VM is visible in Log Analytics via KQL queries.

**Module 3: Use Azure Policy / Machine Configuration to Govern Your Machine**
- **Goal:** Apply and enforce security and compliance policies on Arc-enabled servers using Azure Policy.
- **Actions:**
  - Assign built-in policies for disabling local authentication, enforcing secure TLS protocols, and enabling Microsoft Defender for Cloud.
  - Set policy scope to subscription and include Arc-connected servers.
  - Enable remediation tasks for immediate policy enforcement.
  - Monitor compliance status in the Azure Policy portal.
- **Validation:**
  - Policies are assigned and visible; compliance state is reported in the portal.

**Module 4: Use Microsoft Defender for Cloud to Manage VM Security**
- **Goal:** Monitor and improve the security posture of Arc-enabled VMs using Defender for Cloud.
- **Actions:**
  - Access Defender for Cloud inventory and recommendations for Arc-enabled machines.
  - Review and address security recommendations as needed.
- **Validation:**
  - Arc-enabled VM appears in Defender for Cloud inventory; recommendations are available for review.

**Module 5: Enable Automatic Agent Upgrade**
- **Goal:** Ensure the Azure Connected Machine agent is always up to date via automatic upgrades.
- **Actions:**
  - Enable the Agent auto upgrade (preview) feature in the Arc machine's properties.
  - Refresh the resource page to confirm the setting is enabled.
- **Validation:**
  - Agent auto upgrade status is set to enabled in the Azure portal.
