# Docker Container Lifecycle Management

This document details the standard Docker CLI operations used to monitor, halt, and decommission container instances during application deployment and maintenance workflows.

---

## 🛠️ Command Reference & Operational Impact

| Step | Command | Description & Operational Impact |
| :--- | :--- | :--- |
| **1. Audit Running** | `docker ps` | Lists all currently active, running containers along with their unique Container IDs, image origins, runtime status, and exposed port mappings. |
| **2. Graceful Halt** | `docker stop my-nginx` | Issues a `SIGTERM` signal to safely stop the `my-nginx` process without deleting its underlying container filesystem layer or logs. |
| **3. Audit All** | `docker ps -a` | Displays all containers residing on the host system, including running instances and exited (stopped) containers. |
| **4. Purge Instance** | `docker rm my-nginx` | Permanently removes the stopped `my-nginx` container instance and releases its allocated host resources. |

---

## 🔄 Standard Teardown Workflow

To safely decommission a containerized service, execute the teardown lifecycle in the following sequence:

```bash
# 1. Inspect running containers to verify status and container name
docker ps

# 2. Stop the running process gracefully
docker stop my-nginx

# 3. Confirm the container state updated to 'Exited'
docker ps -a

# 4. Permanently delete the stopped container instance
docker rm my-nginx
