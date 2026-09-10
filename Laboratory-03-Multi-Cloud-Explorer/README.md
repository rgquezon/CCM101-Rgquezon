# Laboratory 3: Multi-Cloud Explorer

## Linux Server Infrastructure Investigation

### System Specifications
* **Operating System:** Ubuntu 24.04.4 LTS (Noble Numbat)
* **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update) @ 2.00GHz
* **CPU Architecture & Cores:** x86_64 (64-bit), 1 CPU Core
* **Memory (RAM):** 1.9 GiB Total (416 MiB Used, 1.5 GiB Available)[cite: 1]
* **Disk Storage:** 19 GiB Root Virtual Disk (`/dev/vda1`, 5.4 GiB Used, 13 GiB Available)[cite: 1]

---

## Cloud Migration Hosting Analysis

Based on this server's resource profile (1 vCPU, 2 GiB RAM, 20 GiB Disk Storage), if this environment were migrated to a public cloud provider, it could be hosted using the following equivalent Infrastructure as a Service (IaaS) compute options[cite: 1]:

1. **Amazon Web Services (AWS):** 
   * **Service:** Amazon EC2 (Elastic Compute Cloud)[cite: 1]
   * **Instance Type:** `t3.small` (2 vCPUs, 2 GiB RAM) or `t4g.small`[cite: 1]
   * **Storage:** 20 GB Amazon EBS General Purpose SSD (gp3)[cite: 1]

2. **Microsoft Azure:** 
   * **Service:** Azure Virtual Machines[cite: 1]
   * **Instance Type:** `Standard_B1ms` (1 vCPU, 2 GiB RAM) or `Standard_B2s`[cite: 1]
   * **Storage:** 32 GB Premium SSD Managed Disk[cite: 1]

3. **Google Cloud Platform (GCP):** 
   * **Service:** Google Compute Engine[cite: 1]
   * **Instance Type:** `e2-small` (2 vCPUs, 2 GiB RAM)[cite: 1]
   * **Storage:** 20 GB Standard / Balanced Persistent Disk[cite: 1]
