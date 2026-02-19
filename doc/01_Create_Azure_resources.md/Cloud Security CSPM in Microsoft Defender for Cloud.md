---
title: 'Cloud Security: CSPM in Microsoft Defender for Cloud'
layout: default
nav_order: 17
parent: 'Lab summaries'
---

**ID** 205727
**Number:** LAB551
**Name:** Cloud Security: CSPM in Microsoft Defender for Cloud
**CloudSubscriptionPoolName:** Microsoft Events 25 - MSLEARN CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

# Cloud Security CSPM in Microsoft Defender for Cloud — Lab Instruction Summary

## Exercise Summary

**Exercise 1: Enabling Defender CSPM Plan**
- **Goal:** Enable and configure Microsoft Defender Cloud Security Posture Management (CSPM) for an Azure subscription.
- **Actions:**
  - Create a Log Analytics workspace in Azure.
  - Enable Defender CSPM and configure monitoring coverage settings (agentless scanning, Kubernetes API access, registry access, sensitive data discovery, permissions management, API security posture management).
  - Link the Log Analytics workspace and enable Foundational CSPM.
- **Validation:**
  - Defender CSPM is enabled and settings are saved; workspace is linked and foundational CSPM is active.

**Exercise 2: Analyzing and Mitigating Attack Paths**
- **Goal:** Use Attack Path analysis to identify and remediate lateral movement risks in cloud environments.
- **Actions:**
  - Access Attack Path analysis in Defender for Cloud.
  - Review attack paths involving internet-exposed VMs and Key Vaults.
  - Use the Remediation tab to address security recommendations.
  - Explore and remediate additional attack paths.
- **Validation:**
  - Attack paths are visualized and remediated; recommendations are applied to reduce risk.

**Exercise 3: Build Query with Cloud Security Explorer**
- **Goal:** Use Cloud Security Explorer to identify and analyze risky resources and vulnerabilities.
- **Actions:**
  - Use predefined and custom queries to find VMs and SQL servers with vulnerabilities or managed identities.
  - Search for storage accounts exposed to the internet or containing sensitive data.
  - Build and refine queries to explore the environment for specific risks.
- **Validation:**
  - Query results display targeted resources and vulnerabilities; findings are actionable.

**Exercise 4: Assign Governance Rule**
- **Goal:** Automate remediation assignment for high-severity vulnerabilities using governance rules.
- **Actions:**
  - Create a governance rule in Defender for Cloud with defined scope, severity, owner, and remediation timeframe.
  - Enable weekly notifications and review the governance report for task status.
- **Validation:**
  - Governance rule is active; remediation tasks are assigned and tracked in the report.

**Exercise 5: Analyze Security Recommendations by Risk Level — Risk Prioritization**
- **Goal:** Prioritize and manage remediation of security recommendations based on risk.
- **Actions:**
  - Access and sort recommendations by risk level in Defender for Cloud.
  - Review high-risk recommendations, analyze details, and assign remediation tasks.
  - Monitor progress through the Governance and Compliance dashboard.
- **Validation:**
  - High-risk vulnerabilities are identified, assigned, and tracked for remediation.

**Exercise 6: Leverage Cloud Identity Entitlement Management — Permissions Management**
- **Goal:** Enable and use Permissions Management (CIEM) to secure cloud identity and access configurations.
- **Actions:**
  - Enable Permissions Management extension in Defender for Cloud.
  - Analyze and adjust permissions across Azure, AWS, or GCP resources.
  - Review new permissions-related recommendations and remediate as needed.
- **Validation:**
  - Permissions Management is enabled; permissions are reviewed and adjusted for least privilege.

**Lab 08: Create an Azure Storage Account and Data Collection Rule (DCR)**
- **Goal:** Deploy infrastructure for centralized log and performance data collection from Azure VMs.
- **Actions:**
  - Deploy an Azure VM, create a storage account, and configure a data collection rule (DCR) with performance counters.
  - Link DCR to Log Analytics workspace and validate data collection setup.
- **Validation:**
  - VM, storage account, and DCR are deployed; data is collected in Log Analytics workspace.

**Lab 09: Configuring Microsoft Defender for Cloud Enhanced Security Features for Servers**
- **Goal:** Enable advanced threat protection for Azure and hybrid servers.
- **Actions:**
  - Enable Microsoft Defender for Servers Plan 2 in Defender for Cloud.
  - Review enhanced security features and plan details.
- **Validation:**
  - Defender for Servers Plan 2 is enabled and active on the subscription.

**Lab 10: Enable Just-in-Time Access on VMs**
- **Goal:** Secure VM access by enabling and managing Just-in-Time (JIT) VM access.
- **Actions:**
  - Enable JIT on VMs, configure access settings, and request access through the portal.
  - Use PowerShell to resolve permission issues if needed.
- **Validation:**
  - JIT access is enabled and tested; access requests are processed as expected.

**Lab 11: Microsoft Sentinel**
- **Goal:** Implement Microsoft Sentinel for threat detection, alerting, and automated response.
- **Actions:**
  - On-board Microsoft Sentinel and connect Log Analytics workspace.
  - Configure Azure Activity data connector and create analytics rules.
  - Deploy a playbook (Logic App) and configure automated responses.
  - Create and test custom alerts, invoke incidents, and review playbook execution.
  - Clean up resources after validation.
- **Validation:**
  - Sentinel is operational; alerts, incidents, and automated responses are triggered and visible in the dashboard.
