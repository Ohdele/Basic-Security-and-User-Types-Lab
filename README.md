<<<<<<< HEAD
# Basic Security and Identifying User Types Lab

Demonstrating foundational Linux system security, user type identification, and auditing tools

## Task 1: Examining /etc/passwd
* **Objective:** Analyze user types (Root, System, Standard) based on the User ID (UID) field in the `/etc/passwd` file.
* **Findings:**
    * **Root User:** Identified by UID **0**.
    * **System Users (Services):** Identified by UIDs **below 1000** (e.g., `daemon:1`, `syslog:104`).
    * **Standard User (Human):** Identified by UIDs starting at **1000** (e.g., `dele:1000`).
