# Automation Research Report

## Core Concepts (Checkpoint 2)

### 1. Bash Script
A Bash script is a plain text file containing a series of Linux commands that the system executes sequentially to automate repetitive tasks. The `#!/bin/bash` line at the very top, known as the shebang, tells the operating system exactly which interpreter (the Bash shell) it must use to execute the code.

### 2. Variables
Programmers use variables (like `$BACKUP_DIR`) to store data such as file paths or configuration settings so they can be easily reused throughout a script. This prevents human errors from typos and makes the script much easier to maintain, as changing the value once at the top of the file automatically updates it everywhere else.

### 3. Cron Job
A cron job is a built-in Linux task scheduler that automatically runs scripts, commands, or software at specific times and intervals. It is essential for cloud operations because it eliminates reliance on human memory, ensuring critical maintenance tasks like nightly backups happen reliably and autonomously at scale.
