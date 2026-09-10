# Lab 03: Multi-Cloud Explorer

## 🚀 The Mission
In this lab, we take our system discovery skills a step further. After auditing our Linux server infrastructure, the goal is to evaluate its resource footprint and map it directly to equivalent hosting options across the "Big Three" public cloud providers: AWS, Azure, and GCP.

## 🖥️ Server Infrastructure Audit
Before mapping to the cloud, we need to know exactly what we are working with. Here is the current resource profile of our Linux instance:

* **Operating System:** Ubuntu 24.04.4 LTS (Noble Numbat)
* **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update) @ 2.00GHz
* **Architecture:** x86_64 (64-bit), 1 vCPU Core
* **Memory (RAM):** 1.9 GiB Total *(416 MiB Used, 1.5 GiB Available)*
* **Disk Storage:** 19 GiB Root Virtual Disk (`/dev/vda1`) *(5.4 GiB Used, 13 GiB Available)*

---

## ☁️ Cloud Migration & Hosting Equivalents
Based on our server's baseline profile (**1 vCPU, ~2 GiB RAM, 20 GiB Storage**), we can determine the most cost-effective Infrastructure as a Service (IaaS) equivalents. 

Here is how this specific machine translates if we were to migrate it to Amazon, Microsoft, or Google's cloud ecosystems:

| Cloud Provider | Compute Service | Target Instance Type | Resource Allocation | Recommended Storage |
|---|---|---|---|---|
| **Amazon Web Services (AWS)** | Amazon EC2 | `t3.small` (or `t4g.small`) | 2 vCPUs, 2 GiB RAM | 20 GB gp3 (General Purpose SSD) |
| **Microsoft Azure** | Azure Virtual Machines | `Standard_B1ms` (or `B2s`) | 1 vCPU, 2 GiB RAM | 32 GB Premium SSD Managed Disk |
| **Google Cloud (GCP)** | Compute Engine | `e2-small` | 2 vCPUs, 2 GiB RAM | 20 GB Standard/Balanced Persistent Disk |

> **💡 Migration Insight:** While our current server only utilizes 1 CPU core, both AWS and GCP's entry-level "small" instances start at 2 vCPUs for the 2 GiB RAM tier. Azure's `Standard_B1ms` is the closest 1:1 hardware match for our exact CPU/RAM ratio, but all three providers offer a seamless, scalable landing zone for this workload.
