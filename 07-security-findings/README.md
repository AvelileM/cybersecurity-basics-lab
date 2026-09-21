# Security Findings

## Overview

This section documents the security observations and lessons learned from the previous investigations in this project.

The goal was not to perform advanced penetration testing, but to identify basic security risks and understand how simple security controls can reduce them.

## Finding 1: File Access Permissions

### Observation

A test file was created inside a private directory.

The directory permissions were changed using:

```bash
chmod 700 private
```

### Security Impact

Before applying the restriction, the directory did not specifically enforce owner-only access.

After applying `chmod 700`, only the owner has:

* Read permission
* Write permission
* Execute/access permission

Group users and other users have no permissions.

### Security Lesson

File permissions are an important access-control mechanism.

Restricting access to files and directories can help prevent unauthorized users from reading or modifying sensitive information.

---

## Finding 2: User and Group Information

### Observation

The project was performed using Git Bash on Windows rather than a native Linux system.

Commands such as:

```bash
id
groups
```

returned Unix-like user and group information, but files such as:

```bash
/etc/passwd
/etc/group
```

were not available.

### Security Lesson

The security commands and their output depend on the operating environment.

It is important to identify the underlying operating system before interpreting security information.

---

## Finding 3: Network Information

### Observation

Basic network investigation was performed using:

```bash
ipconfig
ping
nslookup
```

The tests confirmed that the computer could communicate with external systems and resolve domain names using DNS.

### Security Lesson

Understanding IP addresses, DNS and network connectivity is important when investigating network security.

Network information should also be handled carefully because details such as IP addresses, hostnames and DNS information can reveal information about an environment.

---

## Finding 4: Security Checks

Basic Windows security information was investigated using:

```bash
whoami
whoami /priv
tasklist
netstat -ano
```

These commands can provide information about the current user, privileges, running processes and network connections.

### Security Lesson

Regular security checks can help identify unusual processes, unexpected network connections or excessive privileges.

---

## Overall Lessons

This project demonstrated several basic cybersecurity principles:

* Least privilege
* Access control
* File permissions
* User and group management
* Network awareness
* System investigation
* Security hardening
* Careful handling of system information

The main lesson is that cybersecurity begins with understanding the environment and identifying what should and should not have access to resources.
