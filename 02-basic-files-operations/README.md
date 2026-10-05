# Basic Files Operations

## Objective
Practice essential Linux file system operations from the command line, including navigating directories, creating files and directories, listing files, copying and moving files, renaming files, and removing files and directories.

## Environment
- Platform: LabEx
- Operating System: Linux
- Shell: Bash
- Lab: Basic Files Operations

## Navigating the File System
I practiced determining my current location and navigating between directories.
Commands used:
- pwd — displays the current working directory.
- cd .. — moves to the parent directory.
- cd project — moves into the project directory.
- cd ~ — moves to the user's home directory.
- cd /home/labex/project — navigates using an absolute path.
- echo ~ — displays the user's home directory.
The lab demonstrated the Linux hierarchical file system and the difference between relative and absolute paths.

## Listing Files and Directories
I practiced several variations of the ls command.
Commands used:
- ls — lists files and directories.
- ls -l — displays detailed file information.
- ls -a — displays hidden files.
- ls -la — displays detailed information, including hidden files.
- ls ~ — lists the contents of the home directory.
- ls directory — lists the contents of a specific directory.
- ls -R directory — recursively lists directory contents.
I observed that files beginning with a period, such as .hiddenfile, do not appear when using a standard ls command.

## Creating Files and Directories
I practiced creating files and directories.
Commands used:
- touch file1.txt — creates an empty file.
- echo "Hello, Linux" > file2.txt — creates a file and writes text to it.
- echo "Hidden file" > .hiddenfile — creates a hidden file.
- mkdir testdir — creates a directory.
I used ls and ls -la to verify that the files and directory were created successfully.
## Copying Files and Directories
I practiced copying both individual files and directories.
Commands used:
- cp file1.txt file1_copy.txt — creates a copy of a file.
- cp file2.txt testdir/ — copies a file into a directory.
- cp -r testdir testdir_copy — recursively copies a directory and its contents.
I verified the copied files and directories using ls and by listing the contents of the directories.

## Moving and Renaming Files and Directories
I practiced using the mv command to move and rename files and directories.
Commands used:
- mv file1.txt newname.txt — renames a file.
- mv newname.txt testdir/ — moves a file into a directory.
- mv testdir_copy new_testdir — renames a directory.
- mv testdir/newname.txt ./original_file1.txt — moves a file and changes its name.
This demonstrated that mv can be used for both moving and renaming items.

## Removing Files and Directories
I practiced removing files and directories.
Commands used:
- rm original_file1.txt — removes a file.
- rm -i file2.txt — asks for confirmation before removing a file.
- rmdir testdir — attempts to remove an empty directory.
- rm -r testdir — removes a directory and its contents.
- rm .hiddenfile — removes a hidden file.
- rm -rf temp_dir — recursively and forcefully removes a directory and its contents.
I observed that rmdir cannot remove a directory that still contains files. In that situation, rm -r can be used to remove the directory and its contents.

## What I Learned
This lab gave me hands-on practice with the basic Linux file management commands used to navigate and manage the file system.
I learned how to:
- Navigate using relative and absolute paths.
- Identify my current directory.
- View normal and hidden files.
- Create files and directories.
- Copy files and directories.
- Move and rename files and directories.
- Remove files.
- Remove directories and their contents.
- Use command options such as -a, -l, -R, -r, -i, and -f.

## Security Relevance
File system management is a fundamental Linux skill for cybersecurity and system administration.
Understanding how files and directories are created, copied, moved, renamed, and deleted is important when managing systems, investigating incidents, troubleshooting problems, and working with scripts and configuration files.
Being comfortable with commands such as ls -la, cp, mv, and rm is also important when working from a Linux terminal without a graphical interface.

## Terminal Work
The terminal screenshots document the hands-on commands performed during the lab, including navigating the file system, creating files and directories, viewing hidden files, copying files and directories, moving and renaming items, and removing files and directories.
 
## Lab Completion
The final screenshot documents successful completion of the LabEx Basic Files Operations Lab and the two badges earned from completing the exercise.
 
## Skills Demonstrated
- Linux command-line navigation
- Linux file system structure
- File and directory management
- Hidden file management
- File copying
- Directory copying
- File and directory movement
- File and directory renaming
- File and directory removal
- Bash terminal usage
- Basic Linux administration
## Lab Status
Completed
LabEx badges earned: Starter Skills Badge and Rising Talent Badge.
