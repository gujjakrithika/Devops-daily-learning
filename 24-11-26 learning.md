Today's learning:

## System Management and File Security

# 1. User & Group Account Management
* Identities & Account Types*: Learned how Linux uses **User IDs (UIDs)** and **Group IDs (GIDs)** to control access, and explored the differences between **root**, **regular**, and **service** accounts.
* Account Configuration & Templates*: Understood how user metadata, home directories, and login shells are stored, and how `/etc/skel` provides default template files for newly created accounts.
* Account Lifecycle Security*: Learned best practices for securely locking, disabling, backing up, and removing user accounts while preserving critical data.

# 2. File Permissions, Ownership & Special Bits
* **Standard Permissions (`rwx`)**: Studied read, write, and execute permissions across **user (owner)**, **group**, and **others** using both **symbolic** (`u+x`) and **octal** (`755`) notation.
* **Ownership & Group Collaboration**: Explored how file/directory ownership governs access and how shared directories are configured for secure team collaboration.
* **Special Permissions**: Learned how **SUID**, **SGID**, and the **Sticky Bit** enforce advanced access control on executables and shared directories.

# 3. Process & Job Management
* **Process Monitoring & Control**: Explored Linux process hierarchies (parent-child relationships), identified resource-intensive tasks, and practiced terminating unresponsive processes.
* **Resource Utilization**: Monitored system health across **CPU, memory, and storage**.
* **Job Control**: Learned how Linux manages foreground and background tasks within active shell sessions.

# 4. System Logging & Centralized Monitoring
* **Logging Daemons**: Explored `rsyslog` and `systemd-journald` for tracking system events, auditing activity, and troubleshooting issues.
* **Log Management**: Learned how log messages are categorized, filtered, stored locally, and forwarded to remote logging servers for centralized monitoring.

## Linux Command Line & Shell Scripting

# 5. Using Linux Help Resources
* **Documentation & Pagers**: Learned how to look up command usage with `--help`, `man`, and `info`, and navigated long outputs page-by-page using `less`.
* **Directory Listing Options**: Practiced common `ls` flags including `-l` (long listing), `-a` (hidden files), and `-h` (human-readable sizes) to troubleshoot and learn commands independently.

# 6. Searching & Inspecting Files
* **Fast File Indexing (`locate`)**: Installed `plocate` to quickly find files by name and refreshed the search database using `updatedb`.
* **Content Inspection**: Used `grep` to search inside files, `head` and `tail` to inspect the beginning and end of files, and pipes (`|`) to chain filters.
 * *Key Difference:* `locate` searches for **filenames** via an indexed database, while `grep` searches **inside file contents**.

# 7. Using Linux Network Tools
* **Network Interfaces & IPs**: Used `ip addr` to inspect network configuration, IPv4/IPv6 addresses, loopback (`lo`), and Ethernet interfaces (`ens*`).
* **Ports & Services**: Inspected active network services and listening TCP/UDP sockets using `netstat`.

# 8. Getting Started with Linux Shell Scripting
* **Script Creation**: Built and edited basic shell scripts in **Nano**, starting with the `#!/bin/bash` **shebang** to define the script interpreter and `echo` to display output.
* **Execution Permissions**: Learned why new scripts lack execution permissions by default, applied `chmod +x`, and executed scripts using `./scriptname.sh`.

##  Key Takeaways
* **Defense-in-Depth System Security**: Mastered Linux access control through user/group management, standard `rwx` permissions, and special bits (SUID, SGID, Sticky Bit), alongside `rsyslog` and `journald` auditing.
* **Self-Sufficient CLI Troubleshooting**: Built strong habits for inspecting system state—using built-in documentation (`man`, `--help`), fast file/content search (`locate`, `grep`, `head`, `tail`), and network diagnostics (`ip`, `netstat`).
* **Foundation for Automation**: Combined process/job management with foundational Bash scripting (`#!/bin/bash`, `chmod +x`), bridging manual Linux administration into repeatable DevOps automation.
