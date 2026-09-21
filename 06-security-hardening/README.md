# Basic Security Hardening

## Purpose

The purpose of this exercise is to demonstrate a basic security hardening technique by restricting access to a directory containing sensitive test information.

## Initial Configuration

I created a directory called:

```text
private
```

Inside it I created:

```text
test-data.txt
```

The file contains test information only.

## Initial Permissions

I checked the directory permissions using:

```bash
ls -ld private
```

The initial permissions allowed more access than was required for this test.

## Security Improvement

I changed the directory permissions using:

```bash
chmod 700 private
```

The `700` permission means:

* Owner: read, write and execute
* Group: no permissions
* Others: no permissions

## Testing

After changing the permissions, I tested access using:

```bash
cat private/test-data.txt
```

The file remained accessible to my current user because the user owns the directory.

## What I Learned

I learned that file and directory permissions can be used to reduce unnecessary access to sensitive information.

I also learned that directory permissions affect access to the files contained inside the directory.

## Security Relevance

Restricting access to sensitive files is an important part of system security.

The principle of least privilege means that users should receive only the access they actually need.

In this exercise, the directory was restricted so that only the owner had access.

## Security Principle Demonstrated

**Least Privilege**

Access was restricted to the minimum level required for the owner to work with the test data.

## Next Step

The next exercise will document the security findings from the project and test the security changes made during the lab.
