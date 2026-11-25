Today's Learning:

**Topic:** Networking, Packages, Automation Basics & Linux System Administration Lab

## Networking, Packages, and Automation Basics

### 1. Linux Package & Repository Management
* **Package Managers**: Learned software installation, updates, dependency resolution, and removal using `APT`, `DNF`, and `RPM`.
* **Repository Security**: Explored repository configuration, software sourcing methods, and package verification techniques to maintain reliable Linux systems.

### 2. Networking Fundamentals & Diagnostics
* **Core Networking Concepts**: Studied IPv4 and IPv6 addressing, DNS name resolution, DHCP address allocation, routing, network ports, and common services.
* **Troubleshooting & Security**: Practiced diagnosing connectivity, DNS issues, routes, and active services, while evaluating open ports and service exposure.

### 3. Bash Scripting & Task Automation
* **Shell Variables & Scripting**: Worked with shell/environment variables and built Bash scripts using conditionals, loops, and user input handling to automate repetitive tasks.
* **Task Scheduling**: Studied recurring and one-time job automation using **Cron**, **Systemd Timers**, **At**, and **Batch**.

## Hands-On Lab – Basic Linux system administration

### 1. Monitoring Linux System Processes & Resources
* **`/proc` Virtual File System**: Explored kernel state files and PID directories inside `/proc` (including `/proc/cpuinfo`, `/proc/stat`, and `/proc/meminfo`).
* **System & Process Utilities**: Monitored live CPU/process load with `top`, inspected human-readable RAM/Swap usage with `free -h`, listed running processes with `ps aux`, and checked disk usage with `df -h`.

### 2. Managing Linux Users & Groups
* **Account Databases & Sessions**: Inspected user metadata in `/etc/passwd`, encrypted password hashes in `/etc/shadow`, UID/GID mappings with `id`, and active login sessions with `who`.
* **User Provisioning**: Created a new user with `sudo adduser newstaff` and appended supplementary group memberships using `sudo usermod -aG pslearner newstaff`.

### 3. Checking & Applying File Permissions
* **Permission Inspection**: Created test files (`touch dummyfile`) and analyzed file type and `rwx` permission bits for **owner**, **group**, and **others** using `ls -lah`.
  
