# Mission 6: The Cloud Deployment Engineer

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker%20Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nextcloud](https://img.shields.io/badge/Nextcloud-0082C9?style=for-the-badge&logo=nextcloud&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)

## 📌 Mission Overview
Designed and deployed a multi-tier private cloud storage solution utilizing **Nextcloud** and **MariaDB**, orchestrated through **Docker Compose** as Infrastructure as Code (IaC). This deployment demonstrates service isolation, automated container orchestration, and internal service discovery.

---

## 🎯 Key Objectives
* **Architecture & Service Isolation:** Implement a two-tier containerized architecture separating application logic from relational data storage.
* **Infrastructure as Code (IaC):** Construct and validate a structured `docker-compose.yml` configuration defining services, networks, and environment parameters.
* **Stack Lifecycle Management:** Orchestrate container stack provisioning, status monitoring, and teardown using the Docker Compose CLI.
* **Networking & Service Discovery:** Utilize Docker's internal DNS engine for secure container-to-container communication.

---

## 🛠️ Stack & Architecture

| Tier | Service | Purpose |
| :--- | :--- | :--- |
| **Application Tier** | `Nextcloud` | Enterprise private cloud storage frontend and API |
| **Database Tier** | `MariaDB` | Relational database backend for application metadata |
| **Orchestration** | `Docker Compose` | Infrastructure as Code engine managing the lifecycle |

---

## 📁 Repository Structure
```text
nextcloud-deployment/
└── docker-compose.yml   # Multi-container stack configuration
