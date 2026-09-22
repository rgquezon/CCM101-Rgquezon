# Laboratory 5: The Cloud Data Engineer

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72C48?style=for-the-badge&logo=minio&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

## 📌 Mission Overview
Deploy an S3-compatible **MinIO Object Storage server** using Docker, configure administrative web console access via port forwarding, manage storage buckets, and persist unstructured media assets in a cloud-native sandbox environment.

---

## 🎯 Key Objectives
* **Architectural Foundations:** Differentiate between Block, File, and Object Storage architectures.
* **Containerized Deployment:** Provision an S3-compatible MinIO server using the Docker CLI and Quay.io container registry.
* **Network & Access Control:** Route traffic to cloud service web interfaces using secure port forwarding.
* **Data Management:** Create object storage buckets, set policies, and upload/manage file assets.
* **Technical Documentation:** Document end-to-end cloud storage operations and configurations using Markdown.

---

## 🛠️ Tools & Technologies

| Category | Technology | Operational Role |
| :--- | :--- | :--- |
| **Cloud Environment** | KillerCoda Ubuntu Playground | Ephemeral cloud sandbox for hosting containerized workloads |
| **Container Engine** | Docker CLI & Quay.io Registry | Container runtime execution and repository image pulling |
| **Storage Infrastructure** | MinIO Server & Web Console | High-performance, S3-compatible object storage service |
| **Version Control** | Git & GitHub | Repository management and lab operation tracking |

---

## 🧠 Core Competencies & Skills Learned

* **Container Runtime Management:** Executing containerized storage engines configured with custom port bindings (`-p`), environment variables (`-e`), and storage persistence.
* **S3-Compatible Storage Administration:** Managing object buckets, controlling access, and uploading media assets via modern web dashboards.
* **Cloud Engineering Documentation:** Structuring professional technical guides, system specifications, and operation logs using standard Markdown.

---

## 💡 Architecture Comparison Matrix

| Storage Type | Data Unit | Metadata Capability | Scalability | Primary Use Cases |
| :--- | :--- | :--- | :--- | :--- |
| **Block Storage** | Raw Blocks | Minimal | High | VM Disks, Relational Databases |
| **File Storage** | Files / Hierarchies | Standard File Attributes | Limited | Shared Network Drives, NAS |
| **Object Storage** | Discrete Objects | Unlimited / Custom Key-Value | Elastic (Petabyte+) | Unstructured Media, Data Lakes, Backups |
