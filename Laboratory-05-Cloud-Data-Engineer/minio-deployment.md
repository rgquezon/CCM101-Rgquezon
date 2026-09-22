# MinIO Object Storage Deployment Documentation

## Deployment Configuration
* **Deployment Command:**
* **Web Console Port:** Port `9001` (API service on Port `9000`).
* **Created Bucket Name:** `client-photos`.

## Environment Variables Explanation (`-e` flags)
The `-e` flags pass environment variables into the Docker container process runtime:
* `-e "MINIO_ROOT_USER=cloudadmin"`: Configures the root administrative username for authenticating into the MinIO console and S3 API.
* `-e "MINIO_ROOT_PASSWORD=CloudNova2026!"`: Sets the secure root administrative password.
