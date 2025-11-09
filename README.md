<<<<<<< HEAD
# Basic Security and Identifying User Types Lab

Demonstrating foundational Linux system security, user type identification, and auditing tools

## Task 1: Examining /etc/passwd
* **Objective:** Analyze user types (Root, System, Standard) based on the User ID (UID) field in the `/etc/passwd` file.
* **Findings:**
    * **Root User:** Identified by UID **0**.
    * **System Users (Services):** Identified by UIDs **below 1000** (e.g., `daemon:1`, `syslog:104`).
    * **Standard User (Human):** Identified by UIDs starting at **1000** (e.g., `dele:1000`).
## Task 2: Examining /etc/shadow
* **Objective:** View the sensitive `/etc/shadow` file to locate encrypted password hashes and understand system user locking.
* **Findings:**
    * The **Standard user** (`dele`) contains a **long hashed string** representing the password.
## Task 3: Examining /etc/group and Group Membership
* **Objective:** View the system group database and identify user group memberships using `cat /etc/group`, `groups`, and `id`.
* **Findings:**
    * The `/etc/group` file lists groups and their members (Field 4).
    * The `id` command confirms the user `dele` has UID **1000** and belongs to key groups like **sudo** (granting root access).
