# Linux Permissions & User Management

## What Are Linux Permissions?

Linux permissions control who can access files and directories and what actions they can perform.

There are three types of users:

1. Owner (u) - The user who created the file.
2. Group (g) - Users belonging to the same group.
3. Others (o) - All other users.

There are three permission types:

| Permission | Symbol | Meaning |
|------------|---------|----------|
| Read | r | View file contents |
| Write | w | Modify file contents |
| Execute | x | Run a file as a program |

---

## Viewing File Permissions

### Command

```bash
ls -l
```

### Example Output

```bash
-rw-r--r-- 1 user user 500 May 25 file.txt
```

### Understanding the Output

```bash
-rw-r--r--
```

- First character (-) indicates a regular file.
- rw- means the owner can read and write.
- r-- means the group can only read.
- r-- means others can only read.

Example for a directory:

```bash
drwxr-xr-x
```

- d = directory
- rwx = owner has full permissions
- r-x = group can read and execute
- r-x = others can read and execute

---

## Numeric Permission Values

| Permission | Value |
|------------|--------|
| Read (r) | 4 |
| Write (w) | 2 |
| Execute (x) | 1 |

Examples:

| Permission | Numeric Value |
|------------|--------------|
| rwx | 7 |
| rw- | 6 |
| r-x | 5 |
| r-- | 4 |
| --- | 0 |

---

## Changing Permissions with chmod

### Syntax

```bash
chmod permission filename
```

### Example: chmod 777

```bash
chmod 777 file.txt
```

Permission becomes:

```bash
rwxrwxrwx
```

Everyone has full access.

### Example: chmod 755

```bash
chmod 755 script.sh
```

Permission becomes:

```bash
rwxr-xr-x
```

Owner can read, write, and execute.
Others can read and execute.

### Example: chmod 644

```bash
chmod 644 notes.txt
```

Permission becomes:

```bash
rw-r--r--
```

Owner can read and write.
Others can only read.

---

## Checking Current User

### whoami

Displays the currently logged-in user.

```bash
whoami
```

Example Output:

```bash
sreeja
```

---

## User Information

### id Command

Displays user ID (UID), group ID (GID), and groups.

```bash
id
```

Example Output:

```bash
uid=1000(sreeja) gid=1000(sreeja) groups=1000(sreeja)
```

---

## Creating a New User

### adduser Command

```bash
sudo adduser testuser
```

This command:

- Creates a new user account
- Creates a home directory
- Creates a user group

Example home directory:

```bash
/home/testuser
```

---

## Setting a Password

```bash
sudo passwd testuser
```

Example:

```bash
Enter new UNIX password:
Retype new UNIX password:
```

Password updated successfully.

---

# Hands-On Practice

## Step 1: Create a Directory

```bash
mkdir SecurityLab
```

Verify:

```bash
ls
```

---

## Step 2: Move into the Directory

```bash
cd SecurityLab
```

Check current location:

```bash
pwd
```

---

## Step 3: Create a File

```bash
touch report.txt
```

Verify:

```bash
ls
```

---

## Step 4: Check Permissions

```bash
ls -l
```

Example:

```bash
-rw-r--r-- 1 user user 0 May 25 report.txt
```

---

## Step 5: Change Permissions to 777

```bash
chmod 777 report.txt
```

Verify:

```bash
ls -l
```

Output:

```bash
-rwxrwxrwx
```

---

## Step 6: Change Permissions to 644

```bash
chmod 644 report.txt
```

Verify:

```bash
ls -l
```

Output:

```bash
-rw-r--r--
```

---

## Step 7: Create a Script

```bash
touch script.sh
```

Give execute permission:

```bash
chmod 755 script.sh
```

Verify:

```bash
ls -l
```

Output:

```bash
-rwxr-xr-x
```

---

# Common Interview Questions

## What does ls -l do?

Displays detailed information about files and directories, including permissions.

## What does chmod do?

Changes file or directory permissions.

## What is the meaning of 777?

Everyone has read, write, and execute permissions.

## What is the meaning of 755?

Owner has full permissions. Group and others can read and execute.

## What is the meaning of 644?

Owner can read and write. Group and others can only read.

## What does whoami do?

Displays the current logged-in username.

## What does id do?

Displays the user's UID, GID, and group information.

---

# Practice Commands

```bash
mkdir LinuxPractice
cd LinuxPractice

touch notes.txt
touch script.sh

chmod 644 notes.txt
chmod 755 script.sh

ls -l

whoami
id
```

Expected Results:

- notes.txt → rw-r--r--
- script.sh → rwxr-xr-x

---

# Key Takeaways

- Linux permissions provide security and access control.
- Use ls -l to view permissions.
- Use chmod to change permissions.
- Use whoami to check the current user.
- Use id to view user and group information.
- Use adduser to create new users.
- Use passwd to set or change passwords.
- Understanding permissions is essential for Linux administration and cybersecurity.
