# Container Observability Report

## Application Log Analysis (Checkpoint 4)

### 404 Error Log Line
```text
127.0.0.1 - - [11/Oct/2026:19:30:00 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0"
```
### Importance of Application Logs
Application logs act as essential diagnostic footage for a cloud environment, allowing engineers to trace incoming client requests and pinpoint configuration or routing errors in real time. Without access logs, troubleshooting unexpected error codes like HTTP 404 would require guesswork rather than verifiable evidence.

---

## Real-Time Container Metrics (Checkpoint 5)

* **Container Name:** `client-website`
* **Memory Usage:** `3.2MiB`
* **CPU Percentage:** `0.00%`
