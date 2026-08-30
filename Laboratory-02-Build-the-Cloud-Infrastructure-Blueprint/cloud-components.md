# Cloud Infrastructure Components

## 1. Compute Resources
* **Purpose:** Compute resources provide the processing power and memory required to execute applications, run calculations, and process data.
* **Importance in Cloud Computing:** They allow organizations to rent processing power on-demand and scale up or down based on traffic, eliminating the need to buy and maintain expensive physical servers.
* **Relation to KillerCoda:** In the KillerCoda Linux environment, the compute resources are represented by the CPU and RAM. I interacted with these by running the `lscpu` command to find the CPU model (Intel Xeon) and the `free -h` command to check the allocated memory.

## 2. Storage Resources
* **Purpose:** Storage resources are used to hold, organize, and maintain data, files, and operating system configurations persistently.
* **Importance in Cloud Computing:** Cloud storage provides a highly scalable, secure, and accessible way to keep data safe without relying on local hard drives that can fail or run out of space.
* **Relation to KillerCoda:** The storage in KillerCoda is represented by the virtual disk drives. I viewed these resources by running the `df -h` command, which showed the capacity and usage of the mounted file system (e.g., `/dev/vda1`).

## 3. Networking Resources
* **Purpose:** Networking resources connect servers, storage, and external users, allowing data to be transmitted back and forth across the internet or private networks.
* **Importance in Cloud Computing:** Without networking, cloud resources would be isolated. Networking ensures users can access applications hosted in the cloud quickly and securely from anywhere in the world.
* **Relation to KillerCoda:** The KillerCoda environment is connected to a network that allows me to access the terminal through my web browser. I identified this connection by running the `hostname -I` command, which revealed the server's assigned IP address.

## 4. Operating System
* **Purpose:** The operating system (OS) is the foundational software that manages the hardware resources and provides a platform for running applications and executing commands.
* **Importance in Cloud Computing:** Cloud providers use operating systems (often lightweight Linux distributions) to run virtual machines efficiently, providing a stable and secure environment for users to deploy their software.
* **Relation to KillerCoda:** The operating system running the KillerCoda environment is Ubuntu. I verified this by running `cat /etc/os-release`, which confirmed it is running Ubuntu 24.04 LTS.
