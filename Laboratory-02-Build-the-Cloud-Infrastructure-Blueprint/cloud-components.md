# Cloud Infrastructure Components

## 1. Compute Resources
* **Purpose:** Handles active processing and memory, executing everything from backend system tasks to user applications.
* **Importance in Cloud Computing:** Eliminates the need to maintain physical server hardware. Organizations can provision processing power on demand and scale vCPUs up or down based on real-time traffic spikes.
* **Relation to KillerCoda:** In my terminal session, compute is represented by the virtual CPU and host memory allocation. Running `lscpu` showed an Intel Xeon processor running at 2.0GHz, while `free -h` revealed 1.9GiB of total usable RAM.

## 2. Storage Resources
* **Purpose:** Retains persistent data, application files, and system configs so information isn't lost when instances reboot.
* **Importance in Cloud Computing:** Replaces local hard drives with resilient, scalable virtual disks. This guarantees high data availability, automated snapshots, and hardware failure protection.
* **Relation to KillerCoda:** Storage is represented by virtual block devices attached to the container. Running `df -h` mapped out the active file systems, showing a main 19GiB drive partition (`/dev/vda1`) with 5.4GiB currently in use.

## 3. Networking Resources
* **Purpose:** Connects servers, database backends, and end-users, enabling seamless data flow across private networks and the internet.
* **Importance in Cloud Computing:** Acts as the backbone of cloud architecture. Without proper routing and virtual networks, cloud instances would remain completely isolated and unable to serve web traffic.
* **Relation to KillerCoda:** The sandbox uses a virtual network bridge to route my web browser's terminal input directly to the cloud server. Executing `hostname -I` revealed its assigned internal IP addresses (`172.30.1.2` and `172.17.0.1`).

## 4. Operating System
* **Purpose:** Bridges the physical or virtual hardware with developer applications, managing memory allocation, file systems, and user privileges.
* **Importance in Cloud Computing:** Lightweight Linux distributions serve as the default standard across public clouds due to their low resource overhead, robust CLI automation, and built-in security features.
* **Relation to KillerCoda:** My instance runs a headless Linux distribution. Running `cat /etc/os-release` confirmed Ubuntu 24.04.4 LTS (Noble Numbat), running on kernel version `6.8.0-138-generic`.
