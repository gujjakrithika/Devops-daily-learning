Today's Learning:

# Topics Covered

# 1. Creating, Deleting, and Moving Files
* Practiced core file and directory lifecycle operations in Linux (`touch`, `mkdir`, `cp`, `mv`, `rm`, `rmdir`).
* Managed file organization, renaming, and safe deletion across directories.

# 2. Filtering Data Streams with Wildcards
* Used shell wildcards (`*`, `?`, and character ranges `[ ]`) to match patterns and process multiple files simultaneously.
* Combined wildcards with commands like `ls`, `cat`, `grep`, `sort`, and `wc` for bulk file operations.

# 3. Searching File Systems Using Object Attributes
* Used the `find` command to locate files and directories based on metadata attributes—including **name, file type, size, owner, permissions, and modification date**.
* Distinguished between `find` (searching for file/directory objects) and `grep` (searching inside file contents).

# 4. Ordering Data Using `sort`
* Organized command output alphabetically, in reverse (`-r`), numerically (`-n`), and by unique entries (`-u`).
* Paired `sort` with `uniq` and `wc` to clean and analyze structured output.

# 5. Filtering Data Using `cut` and `wc`
**`cut`**: Extracted specific columns and fields from structured text and data streams using custom delimiters (`-d`, `-f`).
**`wc`**: Counted lines (`-l`), words (`-w`), and characters/bytes (`-c`) to measure and summarize data streams.

# 6. Redirecting Data Streams
* Worked with **Standard Input (`stdin`)**, **Standard Output (`stdout`)**, and **Standard Error (`stderr`)**.
* Redirected command outputs to files using `>` (overwrite) and `>>` (append) to save results and build logs without losing existing data.

# 7. Understanding the Linux System
* **Distribution vs. Kernel**: Learned the difference between a Linux distribution (Ubuntu, Debian, Fedora) and the Linux kernel—the core component managing hardware and system resources.
* **System & Kernel Identification**: Used `uname` / `uname -a` to inspect kernel details and explored OS release metadata stored in `/etc/os-release`.
* **Boot Process & Links**: Examined `/boot` (understanding core boot files like `vmlinuz` and `initrd.img`), practiced shell wildcard (`*`) expansion, and reviewed how symbolic links act as pointers to other files.

# 8. Exploring the Linux File System, Disks & Partitions
 **File System Hierarchy (`/`)**: Explored the root-based directory structure and key system directories:
 * `/boot` – Bootloader and kernel files
 * `/etc` – System configuration files
 * `/home` – User data and home directories
 * `/var` – System logs and variable application data
  **Storage & Partition Management**: Distinguished between physical disks and partitions, and practiced checking mount points, block devices, and disk usage with `lsblk`, `fdisk -l`, and `df -h`.

# 9. Working with Shell & Environment Variables
* **Variable Basics**: Created local shell variables (`OPEN_SOURCE="rocks!"`) and referenced values using the `$` prefix (`echo $VARIABLE_NAME`).
* **Local vs. Environment Scope**: Understood that variables are local to the current shell by default; used `export` to pass variables to child processes (`bash`), `env` to inspect active environment variables, and `unset` to delete variables.

## 💡 Key Takeaways
* **End-to-End CLI Data Processing**: Gained hands-on proficiency in managing files, locating objects (`find`), and filtering, sorting, counting, and redirecting command outputs (`sort`, `cut`, `wc`, `>`, `>>`).
* **Core Linux System Architecture**: Built a solid understanding of how the Linux kernel interacts with distributions, how the standard `/` directory hierarchy is organized, and how to inspect disk partitions and storage usage.
* **Environment & Automation Readiness**: Learned how shell and environment variables (`export`, `env`, `unset`) manage configuration across shell sessions—laying essential groundwork for shell scripting, system administration, and DevOps workflows.
