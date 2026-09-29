# 🐳 Docker Compose Technical Guide

## 🧱 Role of the `services:` Block

The `services:` block defines all the individual containerized applications that make up the multi-tier application stack. Each service entry specifies the base image, environment configurations, container name, and network settings required to run that specific component.

## 📡 Database Discovery (`MYSQL_HOST=database`)

The Nextcloud container locates the MariaDB container through Docker Compose's built-in DNS service discovery. Because both containers are defined in the same `docker-compose.yml` file, Docker Compose automatically creates a shared private network and maps the service name `database` to the container's internal IP address. Setting `MYSQL_HOST=database` allows Nextcloud to communicate directly with MariaDB without hardcoding dynamic IP addresses.

## ⚔️ `docker run` vs `docker-compose up -d`

| ⚙️ Feature | 📦 `docker run` | 🚀 `docker-compose up -d` |
| --- | --- | --- |
| **Execution Model** 🏃 | Manually runs a single container | Deploys multi-container stacks simultaneously |
| **Configuration** 📄 | Command-line flags (`-e`, `-p`, `-v`) | Infrastructure as Code (`docker-compose.yml`) |
| **Network Management** 🌐 | Requires manual network creation and linking | Automatically creates shared container networks |
| **Lifecycle Control** 🔄 | Managed individually container-by-container | Managed as a unified stack (`up`, `down`, `ps`) |
