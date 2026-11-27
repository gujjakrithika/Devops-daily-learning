Today's Learning:

## Hands-On Practice – Linux Users, Groups & File Ownership

### 1. Creating & Managing Groups
* Practiced creating custom Linux groups (`groupadd`) to organize users and simplify shared resource access.
* Verified group definitions, Group IDs (GIDs), and member lists by querying `/etc/group` and `getent group`.

### 2. Provisioning & Maintaining Users
* Practiced creating new user accounts (`useradd -m` / `adduser`), initializing home directories from `/etc/skel`, and setting account passwords (`passwd`).
* Managed group assignments using `usermod -aG` to add users to supplementary groups without overwriting existing memberships, and verified `UID`/`GID` mappings with `id`.

### 3. Managing File & Directory Ownership
* Practiced inspecting file and directory ownership (`ls -ld`, `ls -la`) and modifying owner and group assignments using `chown` and `chgrp`.
* Configured shared directory structures and collaborative group permissions so multiple users within the same group can safely access and manage project files.

## Docker Session
### 1. What is Docker & Why Containers?
* Explored how **Docker** packages applications along with their libraries, dependencies, and runtime configurations into lightweight, portable **containers**.
* Discussed how containers solve environment consistency issues ("it works on my machine") and differ from traditional Virtual Machines by sharing the host OS kernel rather than running a full guest OS per instance.
### 2. Docker Architecture & File System Flow
* **Core Components**: Reviewed the client-server architecture consisting of the **Docker CLI (Client)**, **Docker Daemon (`dockerd`)**, **Docker Images** (read-only templates), **Containers** (running instances), and **Docker Registries** (e.g., Docker Hub).
* **Docker File System & Image Layering Flow**: Discussed how Docker builds images through stacked **read-only layers** (defined via a `Dockerfile`) and attaches a thin **writable container layer** on top at runtime using a Union File System (such as `overlay2`), along with how **Volumes** persist data beyond a container's lifecycle.
