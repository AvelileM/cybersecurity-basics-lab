# Linux File Permissions

## Purpose

The purpose of this exercise is to understand how Linux file permissions control access to files.

## Test Environment

I created a test file called `secret.txt`.

## 1. Create a file

```bash
touch secret.txt
echo "This is a test security file." > secret.txt
```

I used this file to experiment with different permissions.

## 2. Check the original permissions

```bash
ls -l secret.txt
```

The command displayed the permissions assigned to the file.

The permissions are divided into three main categories:

* Owner
* Group
* Others

The permissions can include:

* `r` — read
* `w` — write
* `x` — execute

## 3. Test access

I used:

```bash
cat secret.txt
```

to read the file.

I also used:

```bash
echo "Another line." >> secret.txt
```

to test whether I could modify the file.

Both operations worked because I was the owner of the file and had the required permissions.

## 4. Change the permissions

I changed the permissions using:

```bash
chmod 600 secret.txt
```

The resulting permissions were similar to:

```text
-rw-------
```

This means the owner has read and write access, while the group and other users have no permissions.

## 5. Test the new permissions

I tested the file again using:

```bash
cat secret.txt
```

and:

```bash
echo "Testing permissions." >> secret.txt
```

The commands still worked because I was the file owner and still had read and write permissions.

## What I Learned

I learned that file permissions determine what different users are allowed to do with a file.

The three permission categories are:

* Owner
* Group
* Others

I also learned that `chmod` can be used to change file permissions.

The permission value `600` gives the owner read and write access while giving the group and other users no access.

## Security Relevance

File permissions are important for protecting sensitive information.

Restricting access to only the required users can reduce the risk of unauthorized users reading or modifying files.

## Key Observation

Changing permissions does not necessarily prevent the current owner from accessing a file.

With `600`, the owner still has read and write access.

## Next Step

The next exercise will investigate basic network commands.
