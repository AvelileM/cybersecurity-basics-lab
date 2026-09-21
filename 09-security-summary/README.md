# Security Investigation Summary

## Objective

The objective of this project was to investigate basic cybersecurity concepts using a Windows environment with Git Bash.

The project focused on understanding systems, users, permissions, networking and basic security controls.

## Areas Investigated

### 1. Environment

The operating environment was identified as Windows using Git Bash.

This was important because some Linux commands and files were not available in the same way as they would be on a native Linux system.

### 2. Users and Groups

User and group information was investigated using commands such as:

```bash
whoami
id
groups
```

This demonstrated how user identity and group membership can affect access to system resources.

### 3. File Permissions

File permissions were investigated using:

```bash
ls -l
chmod
```

A test file was created and its permissions were modified.

### 4. Networking

Basic network investigation was performed using:

```bash
ipconfig
ping
nslookup
hostname
```

This demonstrated basic concepts involving IP addresses, DNS and network connectivity.

### 5. Security Checks

Basic system security information was investigated using:

```bash
whoami /priv
tasklist
netstat -ano
```

These commands provided information about privileges, running processes and network connections.

### 6. Security Hardening

A private directory was created and its permissions were restricted using:

```bash
chmod 700 private
```

This demonstrated the principle of least privilege.

## Key Security Principles

The project demonstrated several important cybersecurity principles:

* Least privilege
* Access control
* User identification
* File permissions
* Network awareness
* System monitoring
* Security hardening
* Verification and testing

## What I Learned

The most important lesson was that cybersecurity begins with understanding the environment.

Before securing a system, it is important to understand:

* Who has access?
* What resources exist?
* What permissions are assigned?
* What network connections exist?
* Which processes are running?
* What security controls are already in place?

I also learned that security changes should always be tested after they are applied.

## Conclusion

This project provided practical experience with basic cybersecurity investigation and security controls.

It established a foundation for further learning in areas such as Linux administration, networking, system hardening and cybersecurity.
