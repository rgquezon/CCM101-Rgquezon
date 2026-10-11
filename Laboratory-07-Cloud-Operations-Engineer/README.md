# Mission 7: The Cloud Operations Engineer

## Mission Overview
Established a system performance baseline, deployed a containerized Nginx web server, simulated HTTP traffic, and monitored container access logs and real-time container metrics using Site Reliability Engineering (SRE) observability tools.

## Objectives
* Monitor host CPU, memory, and disk capacity using native Linux CLI tools (`free`, `df`, `top`).
* Deploy an Nginx web server container (`client-website`) and generate simulated user traffic and HTTP errors.
* Extract and examine container access logs to identify successful requests and error codes (HTTP 200 vs HTTP 404).
* Utilize real-time container metrics (`docker stats`) to verify resource efficiency.

## Monitoring Commands Executed
* `free -h`
* `df -h`
* `top`
* `docker run -d -p 8080:80 --name client-website nginx`
* `curl http://localhost:8080`
* `curl http://localhost:8080/hidden-admin-page`
* `docker logs client-website`
* `docker stats`

## Skills Learned
* Host hardware resource auditing and baseline analysis.
* Simulating user traffic and troubleshooting HTTP error codes.
* Container observability, log analysis, and performance metric tracking.
