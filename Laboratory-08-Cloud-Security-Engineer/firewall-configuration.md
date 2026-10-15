# Firewall Configuration Documentation

## Executed Commands

### 1. Allow SSH Access
* `sudo ufw allow ssh`
  
### 2. Configure Default Deny Policy

* `sudo ufw default deny incoming`
* `sudo ufw default allow outgoing`

### 3. Allow Web Traffic (Port 8080)
* `sudo ufw allow 8080/tcp`

## Critical Security Assessment

If `sudo ufw enable` is executed before running `sudo ufw allow ssh`, the firewall will immediately activate with the Default Deny policy, blocking port 22 and instantly locking you out of your remote SSH session.
