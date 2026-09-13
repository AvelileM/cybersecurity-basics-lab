# Linux Users and Groups

## Purpose

The purpose of this exercise is to investigate how users and groups are represented in my command-line environment and understand why they are important for access control.

## Environment

This exercise was performed using Git Bash on Windows.

## Commands Tested

### 1. Check the current user

```bash
whoami
```

### Result

```text
Avelile
```

### What I learned

The `whoami` command identifies the user associated with the current shell session.

---

### 2. Check group membership

```bash
groups
```

### Result

```text
groups: cannot find name for group ID 197610
197610
```

### What I learned

The command attempted to display the groups associated with my current user.

However, Git Bash could not resolve group ID `197610` to a group name and displayed the numeric ID instead.

This appears to be related to the way Git Bash maps Windows user and group information into its Unix-like environment.

This was different from what I expected from a standard Linux system.

---

### 3. Display user and group IDs

```bash
id
```

### Result

```text
uid=197610(Avelile) gid=197610 groups=197610
```

### What I learned

The `id` command displays the current user's UID, GID and group memberships.

My current environment identifies my user as `Avelile` with UID `197610` and GID `197610`.

The output also helps explain the result from the `groups` command because the group ID is displayed as `197610`.

---

### 4. Attempt to view Linux user accounts

```bash
cat /etc/passwd
```

### Result

```text
cat: /etc/passwd: No such file or directory
```

### What I learned

I expected `/etc/passwd` to contain Linux user account information.

The file was not available in my Git Bash environment, showing again that Git Bash does not provide the same filesystem structure as a standard Linux installation.

---

### 5. Attempt to view Linux groups

```bash
cat /etc/group
```

### Result

```text
cat: /etc/group: No such file or directory
```

### What I learned

The standard Linux `/etc/group` file was also unavailable.

This reinforced my understanding that I am working in Git Bash on Windows rather than a native Linux environment.

## Security Relevance

Users and groups are important to cybersecurity because access to files and system resources can be controlled according to user and group permissions.

Understanding who a command is running as and what groups that user belongs to is therefore important when investigating access and permissions.

## Key Observation

The biggest finding from this exercise was that the commands behave differently in Git Bash compared with a standard Linux environment.

I should therefore be careful not to assume that every Unix/Linux command or filesystem path will behave exactly the same way on Windows Git Bash.

## Next Step

The next exercise will investigate file permissions and access control.
