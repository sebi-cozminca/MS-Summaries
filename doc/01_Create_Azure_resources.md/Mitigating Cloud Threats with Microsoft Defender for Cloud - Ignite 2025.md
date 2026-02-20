---
title: 'Mitigating Cloud Threats with Microsoft Defender for Cloud - Ignite 2025'
layout: default
nav_order: 39
parent: 'Lab summaries'
---

**ID** 205062  
**Number:** LAB550  
**Name:** Mitigating Cloud Threats with Microsoft Defender for Cloud - Ignite 2025  
**CloudSubscriptionPoolName:** Microsoft Events 25 - MSLEARN CSS  
**AllowSave:** False   
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Enable Microsoft Defender for Cloud**
- **Goal:** Set up foundational monitoring and enable Microsoft Defender for Cloud protections.
- **Actions:**
  - Create a Log Analytics Workspace for monitoring and integration.
  - Enable Microsoft Defender for Cloud on the subscription and workspace, activating all relevant plans.
  - Review monitoring extensions and protected resources.
  - Explore the Defender for Cloud dashboard for security posture, compliance, and workload protection insights.
- **Validation:**
  - Workspace and Defender plans are provisioned and enabled; dashboard displays active protections and resource coverage.

**Exercise 2: Understanding Microsoft Defender for Cloud Dashboard**
- **Goal:** Explore regulatory compliance, workload protection, and security posture features.
- **Actions:**
  - Review and enable regulatory compliance standards (e.g., ISO 27001:2013, SOC 2 Type 2) in Defender for Cloud.
  - Explore workload protection coverage and recent security alerts.
  - Use inventory and secure score features to assess resource health and compliance.
  - Assign owners and due dates to recommendations for remediation accountability.
- **Validation:**
  - Compliance standards are enabled; workload protection and secure score reflect current environment status; recommendations are assigned and tracked.

**Exercise 3: Explore Secure Score, Recommendations, and Inventory**
- **Goal:** Assess and act on security recommendations to improve cloud security posture.
- **Actions:**
  - Review security recommendations and secure score summary.
  - Download and analyze CSV reports for resource health and recommendations.
  - Filter and investigate specific recommendations (e.g., storage account public access).
  - Explore asset inventory, filter by resource type, and review unhealthy resources and recommendations.
  - Use Azure Resource Graph Explorer to run and save queries for reporting.
  - Review Defender for Cloud pricing and cost estimation workbooks.
  - Explore workload protection dashboards for coverage, alerts, and advanced protection features.
- **Validation:**
  - Secure score and recommendations are visible; reports and queries are generated; inventory and dashboards reflect current security posture.

**Exercise 4: Explore Governance Rules**
- **Goal:** Assign governance rules to drive remediation and accountability for security recommendations.
- **Actions:**
  - Filter recommendations by resource type (e.g., virtual machines).
  - Assign owners and due dates to recommendations using governance rules.
  - Configure notification and remediation timeframe options.
- **Validation:**
  - Governance rules are assigned; recommendations have owners and due dates for follow-up; notifications are configured.
