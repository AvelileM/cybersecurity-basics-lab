# Security Hardening Testing

## Objective

The objective of this test was to verify that the permissions applied to the `private` directory were working as expected.

## Test 1: Check Directory Permissions

Command:

```bash
ls -ld private
```

Expected result:

The directory should have permissions equivalent to:

```text
drwx------
```

This means the owner has read, write and access permissions while group and other permissions are removed.

**Result:** PASS

## Test 2: Access the Directory

Command:

```bash
ls private
```

The directory was accessible by the current user.

**Result:** PASS

## Test 3: Access the Test File

Command:

```bash
cat private/test-data.txt
```

The current user was able to read the test file.

**Result:** PASS

## Security Lesson

The test demonstrated that security controls should be verified after they are applied.

Changing permissions is not enough; the administrator should confirm that the intended user can still access the resource while unnecessary access is restricted.

## Conclusion

The security hardening change was successfully applied and tested.

The `private` directory now follows a more restrictive access model based on the principle of least privilege.
