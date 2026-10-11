# Mission 7 Reflection: The Cloud Operations Engineer

Checking the host server's underlying resources is critical even when containers appear to be running perfectly because all containers share the physical host's CPU, memory, and storage capacity. If the host experiences resource exhaustion, the Linux kernel may intervene and terminate processes unpredictably, crashing healthy containers. 

If a user reports an inability to log into an application, the `docker logs` command serves as primary diagnostic footage by capturing real-time runtime stdout and stderr streams. It allows an engineer to trace incoming HTTP requests, view backend database exceptions, and pinpoint exactly why an authentication request failed. 

There is a fundamental difference between monitoring logs and monitoring metrics. Monitoring logs tracks discrete, text-based historical events and specific error occurrences, whereas monitoring metrics measures live, numerical time-series data such as real-time CPU percentage, memory consumption rates, and network throughput.

Large enterprise companies manage and monitor thousands of distributed containers simultaneously by deploying centralized observability stacks like Prometheus for automated metric scraping and Grafana for visual dashboards, alerting, and telemetry aggregation.

Since starting these laboratory activities, my ability to troubleshoot Linux environments has evolved significantly. I have transitioned from running isolated commands to executing systematic Site Reliability Engineering (SRE) workflows, combining native CLI auditing tools (`free`, `df`, `top`), container access logs, and live metrics to ensure system reliability.
