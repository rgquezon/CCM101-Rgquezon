# Laboratory 02: Build the Cloud Infrastructure Blueprint

## Mission Overview
This laboratory activity focuses on assessing a Linux-based cloud server environment using KillerCoda to evaluate cloud infrastructure components, compare major cloud service providers (AWS, Azure, GCP), design a foundational cloud architecture diagram, and prepare structured technical documentation prior to server deployment.

## Objectives
* Investigate and document key hardware and operating system parameters of a cloud-hosted Linux instance.
* Identify and describe core cloud infrastructure components (Compute, Storage, Networking, OS).
* Compare equivalent cloud services across major public cloud providers.
* Design a simple end-to-end cloud infrastructure diagram for a target application environment.
* Produce professional technical documentation using Markdown and Git version control.

## Cloud Infrastructure Components
* **Compute:** Evaluated processing resources (vCPUs and architecture) utilized for execution workloads.
* **Storage:** Identified block storage allocations, mounted file systems, and available virtual disk capacity.
* **Networking:** Analyzed network interfaces, local/public IP assignments, and routing configurations.
* **Operating System:** Verified Linux distribution release details, kernel versions, and system environment configurations.

## Tools Used
* **KillerCoda Playground:** Cloud-based Linux terminal environment for system discovery.
* **Git & GitHub:** Version control system and remote repository management.
* **Visual Studio Code / Text Editor:** Markdown document preparation and formatting.
* **Diagramming Tool (Draw.io / Excalidraw / Figma):** Architecture diagram generation.

## Linux Commands Executed
* `uname -r` — Checked system kernel version.
* `lsb_release -a` or `cat /etc/os-release` — Verified Operating System details.
* `lscpu` or `cat /proc/cpuinfo` — Inspected CPU model and core count.
* `free -h` — Displayed total and available RAM.
* `df -h` — Displayed disk capacity, usage, and mounted file systems.
* `hostname` — Retrieved the system hostname.
* `ip a` or `ifconfig` — Retrieved network interfaces and IP addresses.

## Skills Learned
* System discovery and environment auditing via Linux command-line tools.
* Mapping physical/virtual Linux host resources to fundamental cloud computing pillars.
* Comparative evaluation of multi-cloud service models across AWS, Azure, and GCP.
* Technical diagramming of user-to-cloud infrastructure workflows.
* Professional documentation formatting adhering to Markdown specifications.

## Challenges Encountered
* Navigating terminal command variations to accurately retrieve specific hardware specifications in a containerized playground environment.
* Aligning service terminology across competing cloud providers (AWS, Azure, GCP) to ensure accurate baseline comparisons.
* Ensuring precise image file paths and directory structures for seamless display within GitHub Markdown previews.
