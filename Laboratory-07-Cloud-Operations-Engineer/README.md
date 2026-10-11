# Mission 7: The Cloud Operations Engineer

## Mission Overview
Established a system performance baseline, deployed a containerized Nginx web server, simulated HTTP traffic, and monitored container access logs and real-time container metrics using Site Reliability Engineering (SRE) observability tools.

## Objectives
* Monitor host CPU, memory, and disk capacity using native Linux CLI tools (`free`, `df`, `top`)[cite: 8, 9].
* Deploy an Nginx web server container (`client-website`) and generate simulated user traffic and HTTP errors[cite: 9, 10].
* Extract and examine container access logs to identify successful requests and error codes (HTTP 200 vs HTTP 404)[cite: 10].
* Utilize real-time container metrics (`docker stats`) to verify resource efficiency[cite: 10].

## Monitoring Commands Executed
* `free -h`[cite: 10]
* `df -h`[cite: 10]
* `top`[cite: 10]
* `docker run -d -p 8080:80 --name client-website nginx`[cite: 10]
* `curl http://localhost:8080`[cite: 10]
* `curl http://localhost:8080/hidden-admin-page`[cite: 10]
* `docker logs client-website`[cite: 10]
* `docker stats`[cite: 10]

## Skills Learned
* Host hardware resource auditing and baseline analysis[cite: 8].
* Simulating user traffic and troubleshooting HTTP error codes[cite: 8].
* Container observability, log analysis, and performance metric tracking[cite: 8].
