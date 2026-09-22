* **Deployment Command:**
  ```bash
  docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
    -e "MINIO_ROOT_USER=cloudadmin" \
    -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
    quay.io/minio/minio server /data --console-address ":9001"
#### 2. Update `README.md`
```bash
cat << 'EOF' > README.md
# Laboratory 5: The Cloud Data Engineer

## Mission Overview
Deploying an S3-compatible MinIO object storage server using Docker, configuring administrative web console access via port forwarding, managing storage buckets, and storing persistent media assets.

## Objectives
* Differentiate between Block, File, and Object Storage architectures.
* Deploy an S3-compatible MinIO Object Storage server using Docker.
* Access a cloud service web interface using port forwarding.
* Create a storage bucket and upload object data.
* Document cloud storage operations using Markdown.

## Tools Used
* KillerCoda Ubuntu Playground
* Docker CLI & Quay.io Container Registry
* MinIO Server & Web Console
* Git & GitHub

## Skills Learned
* Launching containerized storage engines with custom port mappings and environment variables.
* Administering S3-compatible storage buckets and managing unstructured file assets over web dashboards.
* Structuring technical cloud engineering documentation using Markdown.
