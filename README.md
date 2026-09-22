# Cybersecurity Basics Lab

**WTC Project ID:** WTC-ND3P4B9M

## About

This is my Cybersecurity solo project for WeThinkCode_.

The project focuses on practical cybersecurity fundamentals using a Windows computer with Git Bash as the command-line environment.

The goal was to investigate systems, users, permissions, networking and basic security controls through practical exercises.

## Project Goals

* Understand basic cybersecurity concepts
* Investigate users and groups
* Understand file permissions
* Learn basic networking concepts
* Perform basic system security checks
* Apply basic security hardening
* Understand least privilege and access control
* Document security findings
* Use Git and GitHub to track technical work

## Environment

The project was performed on a Windows computer using Git Bash.

This is important because Git Bash provides a Unix-like command-line environment but is not the same as running a native Linux operating system.

Some standard Linux files and commands therefore behaved differently during the investigation.

## Project Structure

```text
cybersecurity-basics-lab/
│
├── README.md
│
├── 01-linux-environment/
│   └── README.md
│
├── 02-users-and-groups/
│   └── README.md
│
├── 03-file-permissions/
│   ├── README.md
│   └── test-data.txt
│
├── 04-network-basics/
│   └── README.md
│
├── 05-security-checks/
│   └── README.md
│
├── 06-security-hardening/
│   └── README.md
│
├── 07-security-findings/
│   └── README.md
│
├── 08-security-testing/
│   └── README.md
│
└── 09-security-summary/
    └── README.md
```

## Investigations

### 01 — Linux Environment

I investigated the command-line environment and learned how to identify:

* Current user
* Working directory
* User and group information
* Available system information

Commands included:

```bash
whoami
pwd
ls
id
```

I also investigated `/etc/os-release` and observed that the standard Linux file was not available because the project was being performed through Git Bash on Windows.

### 02 — Users and Groups

I investigated user and group information using:

```bash
whoami
groups
id
```

This demonstrated the importance of user identity and group membership when controlling access to resources.

### 03 — File Permissions

I investigated file permissions using:

```bash
ls -l
chmod
```

A test file was created and its permissions were changed using:

```bash
chmod 600 test-data.txt
```

This demonstrated how permissions can restrict access to files.

### 04 — Basic Network Investigation

I investigated basic network configuration, connectivity and DNS using:

```bash
hostname
ipconfig
ping
nslookup
```

The investigation demonstrated the relationship between IP addresses, gateways, DNS and network connectivity.

### 05 — Security Checks

I performed basic security checks using:

```bash
whoami
whoami /priv
tasklist
netstat -ano
```

These commands provided information about the current user, privileges, running processes and network connections.

### 06 — Security Hardening

I created a private directory and restricted its permissions using:

```bash
chmod 700 private
```

This demonstrated the principle of least privilege by restricting access to the directory.

### 07 — Security Findings

I documented the security observations from the previous investigations.

Key findings included:

* File permissions can restrict access to resources.
* User and group identity affects access control.
* Network information is important during security investigations.
* System processes and network connections can provide useful security information.
* Security settings should be reviewed and tested after changes.

### 08 — Security Testing

I tested the security hardening changes to confirm that the intended user could still access the protected directory and file.

The testing demonstrated that security controls should be verified after they are applied.

### 09 — Security Summary

The final investigation summary brought together the main cybersecurity concepts explored throughout the project.

## Security Principles

### Least Privilege

Users should have only the permissions required to perform their tasks.

### Access Control

Access to files and resources should be controlled through appropriate permissions and user identities.

### System Awareness

Understanding users, processes, network connections and system configuration is important when investigating security.

### Security Hardening

Reducing unnecessary access and exposure can improve the security of a system.

### Verification

Security changes should be tested to confirm that they work as intended.

## Methodology

Each exercise followed a practical learning process:

```text
Investigate
    ↓
Run commands
    ↓
Observe results
    ↓
Understand what happened
    ↓
Document findings
    ↓
Identify security relevance
    ↓
Test changes
    ↓
Commit changes
```

The goal was to understand the commands and their results rather than simply execute commands without understanding them.

## What I Learned

Through this project I developed practical experience with:

* Command-line environments
* Windows/Git Bash
* Users and groups
* File permissions
* Networking fundamentals
* DNS
* System security checks
* Security hardening
* Access control
* Least privilege
* Troubleshooting
* Technical documentation
* Git and GitHub

## Responsible Use

All security exercises were performed on systems and files that I was authorised to access.

The project focuses on defensive security fundamentals, system administration and controlled experimentation.

Sensitive information such as credentials, private network information and other personal information should not be published in the repository.

## Future Improvements

As my cybersecurity knowledge develops, possible future areas of study include:

* Linux administration
* Log analysis
* Security monitoring
* Network troubleshooting
* Access control
* System hardening
* Cloud security

These areas are outside the scope of this beginner project.

## Project Status

**Completed**

The project has covered basic cybersecurity investigation, access control, networking, security checks, security hardening, findings and testing.

The next stage is to demonstrate the project and explain the practical lessons learned.

## Learning Approach

The project was developed incrementally with genuine Git commits documenting the progression of the work.

The focus was on understanding the relationship between technical actions and their security implications.
