# Cloud-Native Containerization: Docker Fundamentals & Nginx Deployment

A technical lab documentation covering the transition from traditional Virtual Machine (VM) infrastructure to lightweight containerized application environments using Docker.

---

## 📋 Overview & Objectives

This project demonstrates the core principles of containerization, Docker CLI workflow management, and cloud-native application deployment using a KillerCoda cloud environment.

### Learning Objectives
* **Infrastructure Concepts:** Differentiate between traditional Virtual Machines (VMs) and lightweight Linux containers.
* **Environment Provisioning:** Access and utilize a Docker-enabled cloud environment (KillerCoda).
* **CLI Operations:** Master fundamental Docker CLI commands for container lifecycle management.
* **Application Deployment:** Pull, execute, expose, inspect, and terminate an Nginx web server container.
* **Documentation & Version Control:** Maintain structured Markdown documentation and resolve environment state resets using Git workflows.

---

## 🛠️ Command Reference & Operational Workflow

| Step | Command | Purpose / Description |
| :--- | :--- | :--- |
| **1. Verification** | `docker --version` | Verified local Docker engine installation and CLI version. |
| **2. System Check** | `docker info` | Inspected system-wide Docker operational status and container stats. |
| **3. Image Retrieval** | `docker pull nginx` | Downloaded the official Nginx base image from Docker Hub repository. |
| **4. Deployment** | `docker run -d -p 8080:80 --name my-nginx nginx` | Deployed Nginx in detached mode (`-d`) mapping host port 8080 to container port 80. |
| **5. Testing** | `curl http://localhost:8080` | Verified local HTTP web server response and accessibility. |
| **6. Monitoring** | `docker ps` | Listed currently active and running container processes. |
| **7. Termination** | `docker stop my-nginx` | Safely halted the execution of the running Nginx container. |
| **8. Audit** | `docker ps -a` | Verified the stopped state of all container instances. |
| **9. Cleanup** | `docker rm my-nginx` | Permanently removed the stopped container instance from the host system. |

---

## 🔑 Key Core Concepts Learned

* **Container Lifecycle Management:** Gained hands-on experience controlling container states across the complete lifecycle: image pulling, instantiation (`run`), inspecting status (`ps`), stopping, and removing instances.
* **Port Forwarding & Namespace Isolation:** Understood how host-to-container port mapping (`-p 8080:80`) bridges isolated network namespaces with host interfaces.
* **Cloud-Native Documentation:** Standardized technical Markdown documentation procedures for reproducibility in cloud infrastructure environments.

---

## 💡 Troubleshooting & Lessons Learned

### Handling Ephemeral Environment Resets
* **Issue:** Session resets in cloud sandbox environments like KillerCoda often cause Git remote branch synchronization mismatches.
* **Solution:** Resolved out-of-sync local histories cleanly by executing `git pull --rebase` prior to committing new documentation.

### Isolated Container Networking
* Containers run in isolated network environments by default. Services exposed inside the container (e.g., Nginx default port `80`) remain inaccessible to external clients unless explicitly bound to a host port using `-p <host_port>:<container_port>`.
