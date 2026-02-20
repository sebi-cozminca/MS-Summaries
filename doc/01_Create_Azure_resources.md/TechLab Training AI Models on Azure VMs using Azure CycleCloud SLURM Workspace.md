---
title: 'TechLab: Training AI Models on Azure VMs using Azure CycleCloud SLURM Workspace'
layout: default
nav_order: 80
parent: 'Lab summaries'
---

**ID** 170870  
**Number:** 41-411-2  
**Name:** TechLab: Training AI Models on Azure VMs using Azure CycleCloud SLURM Workspace  
**CloudSubscriptionPoolName:** CycleCloud CSS (Recycling)  
**AllowSave:** False  
**CloudCredentialPoolAssignments:** NA  
**Additional licenses:** NA  

---

## Exercise Summary

**Exercise 1: Deploy Slurm Workspace using a marketplace image**
- **Goal:** Deploy and configure an Azure CycleCloud Workspace for Slurm, including all required infrastructure.
- **Actions:**
  - Create an SSH key for deployment.
  - Deploy Azure CycleCloud Workspace for Slurm from the Azure Marketplace with custom VM and partition settings.
  - Install Azure CLI and Azure Bastion extension.
  - Establish Bastion tunnels and access the CycleCloud web app.
  - (If needed) Manually add a login node to the cluster.
  - Review and validate cluster and node settings in the CycleCloud web app.
- **Validation:**
  - Cluster and nodes are visible and in the ready state in the CycleCloud web app; login node resource ID and GPU node name are recorded.

**Exercise 2: Add a GPU node to the cluster and perform NCCL testing**
- **Goal:** Add a GPU node, perform NCCL performance tests, and verify container support on the cluster.
- **Actions:**
  - Connect to the login node via SSH and Bastion.
  - Clone required GitHub repositories (cyclecloud-llm, AI_on_Infra_Lab).
  - Add a GPU node using Slurm and validate its readiness.
  - Create a tunnel for VS Code SSH access and connect to the login node.
  - Run a baseline NCCL test (without Slurm) and a batch NCCL test (with Slurm), comparing results.
  - Verify container support by running a PyTorch container and checking torch version output.
- **Validation:**
  - Successful NCCL test results are produced and compared; container test outputs torch version; job logs are available in VS Code.

**Exercise 3: Load test dataset and run sentiment analysis (inference) with DistilBERT**
- **Goal:** Benchmark and run inference using DistilBERT on the cluster with a sample movie review prompt.
- **Actions:**
  - Prepare and edit the inference script and job submission file in VS Code.
  - Submit a Slurm batch job for benchmarking and inference.
  - Monitor job completion and review output files for sentiment prediction results.
- **Validation:**
  - Output files (bert_inference.err, bert_inference.out) are generated and show the sentiment prediction for the provided prompt.

**Lab Completion**
- **Validation:**
  - Submit the lab in the Skillable platform and confirm completion status in Viva and Learning Path the following week.
