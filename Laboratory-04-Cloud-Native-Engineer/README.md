Transitioning from traditional Virtual Machine infrastructure to lightweight containerized application environments using Docker.
* Differentiate between traditional Virtual Machines (VMs) and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate a containerized Nginx application.
* Create professional technical documentation of container operations using Markdown.
* `docker --version` - Verified Docker installation and CLI version.
* `docker info` - Checked system-wide Docker operational status.
* `docker pull nginx` - Downloaded official Nginx image from Docker Hub.
* `docker run -d -p 8080:80 --name my-nginx nginx` - Deployed Nginx container in detached mode with host-to-container port mapping.
* `curl http://localhost:8080` - Tested local HTTP web server availability.
* `docker ps` - Listed active, running containers.
* `docker stop my-nginx` - Halted running Nginx container process.
* `docker ps -a` - Verified stopped status across all containers.
* `docker rm my-nginx` - Permanently deleted stopped container instance.
* Container lifecycle management (pull, run, inspect, stop, remove).
* Port forwarding between host network interfaces and isolated container namespaces.
* Technical Markdown documentation for cloud-native workflows.
* Resolving Git remote sync mismatches (`git pull --rebase`) when terminal sessions reset in KillerCoda.
* Understanding isolated container networking and exposed ports (`-p 8080:80`).
