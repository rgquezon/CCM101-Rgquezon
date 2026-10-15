# Mission 8: The Cloud Security Engineer

## Mission Overview
Implemented host-based firewall security on an Ubuntu cloud server using Uncomplicated Firewall (UFW) to enforce the Principle of Least Privilege and reduce the system's attack surface.

## Objectives
* Understand the Attack Surface and Principle of Least Privilege (PoLP).
* Deploy a containerized web application (`secure-web-app`) exposed on port 8080.
* Configure UFW with a Default Deny policy for incoming traffic.
* Implement granular port rules to selectively allow SSH (Port 22) and HTTP (Port 8080).

## Commands Executed
* `docker run -d -p 8080:80 --name secure-web-app nginx`
* `sudo ufw allow ssh`
* `sudo ufw default deny incoming`
* `sudo ufw default allow outgoing`
* `sudo ufw enable`
* `sudo ufw status verbose`
* `sudo ufw allow 8080/tcp`
* `sudo ufw status numbered`
* `curl http://localhost:8080`

## Skills Learned
* Host-based network perimeter control and firewall administration.
* Applying Default Deny rules to systematically restrict network intrusion vectors.
* Granular service enablement without compromising underlying server accessibility.
