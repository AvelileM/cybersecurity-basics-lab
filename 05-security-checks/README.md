# Basic Security Checks

## Purpose

The purpose of this exercise is to perform basic security checks on my Windows environment and understand what information can be gathered about the current system.

## 1. Current User

### Command

```bash
whoami
```

### Result

The command identified the account currently running the shell.

### What I Learned

The current user is important when investigating system access because permissions and privileges are associated with user accounts.

## 2. User Privileges

### Command

```bash
whoami /priv
```

### What I Observed

The command displayed privileges associated with the current Windows account.

### What I Learned

Windows uses privileges to control what certain accounts or processes are allowed to do.

I learned that having an account does not automatically mean that every possible system operation is available to it.

## 3. Running Processes

### Command

```bash
tasklist
```

### What I Observed

The command displayed processes currently running on the system.

### What I Learned

Running processes represent programs or system components currently executing.

Viewing running processes can be useful when investigating unusual system activity.

## 4. Network Connections

### Command

```bash
netstat -ano
```

### What I Observed

The command displayed network connections and listening ports along with process IDs.

### What I Learned

Network connections can be associated with processes using their process IDs.

This can help investigators understand which processes are communicating over the network.

## Security Relevance

These checks demonstrate how basic system information can be gathered during a security investigation.

Understanding the current user, privileges, running processes and network connections provides useful information about the state of a system.

## Important Observation

This investigation was performed on my own Windows computer.

The project does not involve scanning or accessing systems that I do not own or have permission to investigate.

## Next Step

The next exercise will build on these checks by identifying potential security issues and investigating basic security hardening.
