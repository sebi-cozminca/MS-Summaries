---
title: 'Modernize your Open Source Linux Workloads Prod [OLD VERSION]'
layout: default
nav_order: 40
parent: 'Lab summaries'
---

**ID** 186388  
**Number:** LAB313  
**Name:** Modernize your Open Source Linux Workloads Prod [OLD VERSION]  
**CloudSubscriptionPoolName:** Microsoft CSU CSS - Recycling (Prod)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** TrialFabricUsers  

---

## Exercise Summary

**Exercise 1: Convert CentOS 7 VM to RHEL 7**
- **Goal:** Migrate a CentOS 7 system to Red Hat Enterprise Linux 7 using Convert2RHEL.
- **Actions:**
  - Connect to the CentOS VM via Hyper-V and SSH.
  - Update system repositories to CentOS Vault and perform system update.
  - Enable and configure the Convert2RHEL repository and install the utility.
  - Set environment variables to bypass kernel/module checks for lab use.
  - Run Convert2RHEL with activation key and reboot into RHEL kernel.
  - Verify conversion, enabled repositories, and review conversion logs.
- **Validation:**
  - System reports as RHEL 7, CentOS repos are removed, and conversion logs show success.

**Exercise 2: Connect RHEL VM to Azure Arc**
- **Goal:** Onboard the converted RHEL VM to Azure Arc for hybrid management.
- **Actions:**
  - Create or use an existing Azure resource group for Arc.
  - Generate and download the Azure Arc onboarding script from the portal.
  - Install required tools, save, and run the script on the VM.
  - Authenticate with Azure using device login.
- **Validation:**
  - VM appears as an Arc-enabled server in the Azure portal resource group.

**Exercise 3: Set Up PostgreSQL Server and Import Database**
- **Goal:** Deploy and configure a PostgreSQL server on CentOS and import a sample database.
- **Actions:**
  - Connect to the PostgreSQL VM, set hostname, and install nano.
  - Download and run setup script for PostgreSQL.
  - Create and connect to the northwind database, import schema, and verify tables.
  - Modify PostgreSQL configs for remote access and set user password.
  - Restart PostgreSQL service.
- **Validation:**
  - Database is accessible, tables are present, and remote connections are enabled.

**Exercise 4: Set Up Apache Web Server**
- **Goal:** Deploy Apache on CentOS and configure it to connect to PostgreSQL.
- **Actions:**
  - Connect to the Apache VM, set hostname, and install nano.
  - Download and run setup script for Apache.
  - Download and edit sample PHP file to use correct DB connection details.
  - Test web page and troubleshoot SELinux denials using audit2allow.
  - Set SELinux booleans to allow Apache-PostgreSQL connectivity.
- **Validation:**
  - Web page loads and connects to the PostgreSQL database successfully.

**Exercise 5: Migrate PostgreSQL Database to Azure**
- **Goal:** Migrate the on-premises PostgreSQL database to Azure Database for PostgreSQL Flexible Server.
- **Actions:**
  - Create Azure resource group, public IP, and PostgreSQL Flexible Server via Azure portal.
  - Configure firewall rules and gather connection info.
  - Dump local northwind database and create/restore it on Azure PostgreSQL.
  - Update Apache PHP app to point to Azure database and verify connectivity.
- **Validation:**
  - Azure PostgreSQL contains the migrated database; web app connects to Azure DB and functions as expected.
