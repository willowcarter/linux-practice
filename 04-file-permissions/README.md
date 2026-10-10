# LabEx: Permissions of Files

## Objective

Learn how to inspect and modify Linux file permissions, change file and directory ownership, create nested directories, and grant execute permissions to a Bash script.

## Commands Used

### 1. Create and Inspect Files

```bash
cd ~/project
touch example.txt
ls -l example.txt
```

- `touch` creates an empty file if it does not exist.
- `ls -l` displays file permissions, ownership, size, and modification time.

### 2. Change File Ownership

```bash
sudo chown root:root example.txt
ls -l example.txt
```

- `chown` changes file ownership.
- `root:root` specifies the root user as the owner and the root group as the group.
- `sudo` runs the command with elevated privileges.

### 3. Create Nested Directories and Files

```bash
mkdir -p new-dir/subdir
echo "Hello, world" > new-dir/file1.txt
echo "Another file" > new-dir/subdir/file2.txt
ls -lR new-dir
```

- `mkdir -p` creates a directory structure, including parent directories.
- `echo` outputs text.
- `>` writes output to a file, replacing existing contents.
- `ls -lR` recursively lists directory contents and displays detailed information.

### 4. Change Ownership Recursively

```bash
sudo chown -R root:root new-dir
ls -lR new-dir
```

- The `-R` option applies the ownership change recursively to the directory and its contents.
- The listing verifies the updated ownership of the files and subdirectory.

### 5. Create and Execute a Bash Script

Create the script:

echo '#!/bin/bash' > script.sh
echo 'echo "Hello, World"' >> script.sh
cat script.sh

Inspect its permissions:

ls -l script.sh

Attempting to run the script initially returned a permission-denied error because the file did not have execute permission.

Grant execute permission to the file owner:

chmod u+x script.sh
ls -l script.sh
./script.sh

The script then executed successfully and printed:

Hello, World

What I Learned

Linux permissions determine who can read, write, and execute files.

The r, w, and x characters represent read, write, and execute permissions.

ls -l displays permissions and ownership information.

chown changes the owner and group of a file or directory.

chown -R applies ownership changes recursively.

chmod u+x adds execute permission for the file owner.

mkdir -p creates nested directory structures.

The > operator overwrites a file, while >> appends to it.

A Bash script can contain a shebang such as #!/bin/bash to identify its interpreter.

A script needs execute permission to run directly using ./script.sh.

Security Relevance

Correct file permissions and ownership help prevent unauthorized access and modification. Granting only the permissions required for a task supports the principle of least privilege. Recursive ownership changes and commands run with sudo should be used carefully because they can affect many files and system resources.

Evidence

creating-files-and-setting-ownership.png — Creating a file, inspecting permissions, and changing ownership.

changing-ownership-recursively.png — Changing ownership recursively and verifying the results.

adding-execute-permission-to-script.png — Creating a Bash script, troubleshooting a permission-denied error, granting execute permission, and running the script.

Status

Completed — Permissions of Files Lab.
