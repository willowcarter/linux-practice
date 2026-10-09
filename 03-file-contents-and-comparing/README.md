# LabEx: File Contents and Comparing

## Objective
Practice viewing file contents, displaying specific lines or characters, and comparing two files using Linux terminal commands.

## Commands Used
- `cat /tmp/hello` — Display the contents of a file.
- `cat -n /tmp/hello` — Display file contents with line numbers.
- `head -n1 /tmp/hello` — Display the first line.
- `head -c1 /tmp/hello` — Display the first byte.
- `tail -n1 /tmp/hello` — Display the last line.
- `tail -c1 /tmp/hello` and `tail -c2 /tmp/hello` — Display the last one or two bytes.
- `cd ~/project` — Change to the project directory.
- `diff file1 file2` — Compare two files and display their differences.

## What I Learned
- `cat` displays file contents and can number lines with the `-n` option.
- `head` and `tail` display the beginning and end of files.
- The `-n` option specifies a number of lines, while `-c` specifies a number of bytes.
- `diff` compares files line by line and identifies changes.
- In `diff` output, `<` indicates content from the first file, and `>` indicates content from the second file.
- The notation `1c1` indicates that line 1 in the first file differs from line 1 in the second file.

## Security Relevance
These commands are useful for inspecting configuration files, reviewing logs, and comparing file versions to identify unexpected changes. File comparison is a helpful basic technique for troubleshooting and investigating potential configuration modifications.

## Evidence
- `screenshot.png` — Terminal commands and output demonstrating file inspection and comparison.

## Status
Completed — File Contents and Comparing Lab. Earned the Lab Explorer badge.
