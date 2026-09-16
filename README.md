# Cybersecurity Basics Lab

A beginner-friendly cybersecurity project focused on Linux fundamentals, system administration, networking, access control, and basic security practices.

This project documents my practical learning journey as I build foundational cybersecurity skills.

## About the Project

The purpose of this project is to develop practical cybersecurity knowledge by investigating and documenting fundamental concepts rather than only studying theory.

Each section contains commands, observations, explanations, and security relevance based on practical exercises.

The project is being completed using a Windows computer with Git Bash as the current command-line environment.

## Learning Objectives

Through this project, I aim to develop an understanding of:

* Linux and Unix-like environments
* Users and groups
* File permissions
* Basic networking
* System security checks
* Security hardening
* Access control
* Security documentation
* Basic troubleshooting
* Git and GitHub for documenting technical work

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
│   └── README.md
│
└── 04-network-basics/
    └── README.md
```

## Completed Investigations

### 01 — Linux Environment

Investigated the command-line environment and learned how to identify the current user, working directory, and basic system information.

Commands explored include:

```bash
whoami
pwd
ls
id
cat /etc/os-release
```

An important observation was that the project is currently being performed through Git Bash on Windows rather than a native Linux installation. This affects which Linux files and commands are available.

---

### 02 — Users and Groups

Investigated how users and groups are represented in the command-line environment.

Commands explored include:

```bash
whoami
groups
id
cat /etc/passwd
cat /etc/group
```

The exercise demonstrated the importance of user and group identity in access control.

Some standard Linux files were unavailable because the current environment is Git Bash on Windows.

---

### 03 — File Permissions

Investigated file permissions and how they control access to files.

The exercise explored:

```bash
ls -l
chmod
```

A test file was created and its permissions were changed using:

```bash
chmod 600 secret.txt
```

This demonstrated how permissions can be used to restrict access to sensitive files.

---

### 04 — Basic Network Investigation

Investigated basic network configuration, connectivity and DNS.

Commands explored include:

```bash
hostname
ipconfig
ping
nslookup
```

The investigation demonstrated how IP addresses, gateways, DNS and network connectivity are related.

It also showed that command syntax can differ between Windows and Linux environments.

## Security Concepts

The project currently focuses on the following fundamental security concepts:

### Identity

Understanding which user account is operating a system or command-line session.

### Access Control

Understanding how users, groups and permissions determine access to resources.

### Least Privilege

Giving users only the access they need can reduce unnecessary access to system resources.

### Network Awareness

Understanding basic IP addressing, DNS, gateways and connectivity is important when investigating network-related problems.

### Security Hardening

Future exercises will investigate basic methods of reducing unnecessary exposure and improving system security.

## Methodology

Each investigation follows a practical learning process:

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
Commit changes
```

The goal is not simply to execute commands, but to understand why they are being used and what their results mean.

## Git Workflow

Git is used to track the development of this project.

Each completed investigation is committed separately so that the project history shows the progression of my learning.

Example:

```bash
git add .
git commit -m "Document basic network investigation"
git push
```

## Responsible Use

All security exercises in this repository are performed on systems and files that I am authorised to access.

The project focuses on defensive security fundamentals, system administration and controlled experimentation.

Sensitive information such as private IP addresses and other personally identifying network information should not be published in the repository.

## Current Progress

* [x] Linux environment investigation
* [x] Users and groups investigation
* [x] File permissions investigation
* [x] Basic network investigation
* [ ] Basic security checks
* [ ] Security hardening
* [ ] Document security findings
* [ ] Test security changes
* [ ] Improve project documentation
* [ ] Create project demonstration

## Skills Being Developed

* Linux command line
* Windows/Git Bash
* File permissions
* Users and groups
* Networking fundamentals
* DNS fundamentals
* Basic system security
* Troubleshooting
* Technical documentation
* Git
* GitHub

## Future Improvements

As my cybersecurity knowledge improves, this project will be expanded with additional practical exercises covering areas such as:

* System security checks
* Network troubleshooting
* Security configuration
* Access control
* Log analysis
* Basic security monitoring
* Linux administration

The complexity of the exercises will increase as I develop a stronger understanding of the fundamentals.

## Learning Goal

The long-term goal of this project is to build a practical foundation for pursuing further studies and entry-level opportunities in cybersecurity, Linux/system administration, cloud security and related technology roles.
