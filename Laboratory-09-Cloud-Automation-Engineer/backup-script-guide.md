# Backup Script Guide

## 1. Automation Script Code
```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")
echo "Initiating automated backup..."
mkdir -p $BACKUP_DIR
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR
echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. Permissions Explanation
The command `chmod +x backup.sh` modifies the file's permissions to make it an executable program. By default, Linux prevents plain text files from running to protect the system. The `+x` (execute) flag explicitly grants the operating system permission to run the script.

## 3. Cron Schedule Breakdown
**Cron Expression:** `0 2 * * * /root/backup.sh`
* **0** (Minute): Runs exactly at minute 0.
* **2** (Hour): Runs at 2 AM (02:00).
* **\*** (Day of Month): Runs every day of the month.
* **\*** (Month): Runs every month.
* **\*** (Day of Week): Runs every day of the week.
