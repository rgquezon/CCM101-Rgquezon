# Lab 02: Building the Cloud Infrastructure Blueprint

## 🚀 The Mission
In this lab, we roll up our sleeves and dive into a live Linux-based cloud server using KillerCoda. The main goal? To peek under the hood and understand exactly what makes a cloud environment tick. 

We’ll audit the system's hardware and OS, break down the core pillars of cloud infrastructure, and compare how the "Big Three" providers (AWS, Azure, and GCP) handle these services. Finally, we'll map everything out in a clean, professional architecture diagram before getting it all documented and pushed via Git.

## 🎯 What We Set Out to Do
* **Audit the System:** Explore a cloud-hosted Linux instance to document its hardware and OS parameters.
* **Deconstruct the Cloud:** Identify the core infrastructure pillars (Compute, Storage, Networking, OS) running on the machine.
* **Translate the Providers:** Compare equivalent cloud services across AWS, Azure, and Google Cloud Platform.
* **Visualize the Architecture:** Sketch out a simple, end-to-end cloud infrastructure diagram for a target app.
* **Write Like a Pro:** Produce clean, readable technical documentation using Markdown and Git.

## 🏗️ Under the Hood: Core Components
During our system audit, we mapped out the foundational pieces of our cloud environment:
* **Compute:** Looked at the actual "brains" of the operation, checking out the vCPUs and architecture powering our workloads.
* **Storage:** Investigated our block storage, saw how the file systems were mounted, and checked our available virtual disk capacity.
* **Networking:** Traced how the server talks to the outside world by pulling network interfaces, local/public IPs, and routing setups.
* **Operating System:** Confirmed exactly what flavor of Linux we were running, down to the kernel version and environment config.

## 🛠️ The Toolkit
* **KillerCoda Playground:** Our sandbox. A cloud-based Linux terminal perfect for safely running discovery commands.
* **Git & GitHub:** For version control and keeping our documentation backed up and accessible.
* **VS Code:** The trusty editor for writing and formatting this Markdown file.
* **Draw.io / Excalidraw:** To bring our architecture diagram to life.

## 💻 Commands We Relied On
We used built-in Linux tools to interrogate the system. Here are the main commands that got the job done:

* `uname -r` — Checked the exact system kernel version.
* `cat /etc/os-release` — Verified the specific Linux distribution details.
* `lscpu` — Popped the hood on the CPU to check the model and core count.
* `free -h` — Displayed how much RAM we had to play with (in a human-readable format).
* `df -h` — Showed our disk capacity, current usage, and mounted file systems.
* `hostname` — Grabbed the system's designated name.
* `ip a` — Listed out all network interfaces and assigned IP addresses.

## 🧠 Biggest Takeaways
* **System Discovery:** Got much more comfortable exploring a mystery Linux environment using just the command line.
* **Connecting the Dots:** Learned how to map a virtual machine's standard resources back to fundamental cloud computing concepts.
* **Multi-Cloud Fluency:** Figured out how to speak the language of AWS, Azure, and GCP interchangeably.
* **Visual Communication:** Practiced sketching out user-to-cloud workflows in a way that actually makes sense to a reader.
* **Docs as Code:** Leveled up professional documentation skills using Markdown specifications.

## 🚧 Roadblocks & Troubleshooting
* **Command Quirks:** Figuring out which commands worked best in a containerized playground, as some standard Linux commands behave slightly differently in KillerCoda.
* **Cloud Translation:** It was initially tricky remembering all the naming conventions—like how AWS calls it an EC2, Azure calls it a VM, and GCP calls it a Compute Engine!
* **Markdown Images:** Wrestling with relative image file paths in GitHub. It took a little trial and error to ensure the architecture diagram actually loaded in the preview instead of showing a broken link.
