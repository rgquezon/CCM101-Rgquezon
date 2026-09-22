# Cloud Storage Types Comparison Report

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Stores data in raw, unformatted, fixed-size volumes (blocks). Operates like a virtual hard drive attached to a single VM. | Operating system boot drives, relational databases, and high-performance transactional workloads. | AWS EBS (Elastic Block Store), Azure Managed Disks |
| **File Storage** | Stores data in a hierarchical file and folder tree structure shared across multiple network devices. | Centralized enterprise file shares, content management systems, and legacy app data sharing. | AWS EFS (Elastic File System), Azure Files |
| **Object Storage** | Stores data as discrete objects in flat buckets paired with unique IDs and rich custom metadata over HTTP APIs. | Storing massive volumes of unstructured data like images, video streaming files, and system backups. | AWS S3 (Simple Storage Service), Google Cloud Storage |

---

## Client Recommendation: User Image Storage

Object Storage is the ideal architecture for your photo-sharing application because it stores unstructured data in a flat namespace without the overhead of hierarchical file systems. Unlike Block Storage attached to a specific server, Object Storage scales infinitely, allowing you to store millions of user images seamlessly via HTTP REST APIs. Additionally, because web containers are ephemeral, offloading image uploads to Object Storage ensures user files remain safely persistent and accessible even when web containers restart.
