# Bandit - Level 5

## Objective
The goal of this level is to find the password for Level 5. The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable


## Steps
1. Open the terminal.
2. Connect to the server using SSH:

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```
3. Enter the password for level 4
4. List all files list files including hidden ones (ls -a), locate the hidden file, and read its content using commands like cat, less, or more to find the password for the next level.
```bash
ls -a
```
5. Locate the Directory named inhere.
```bash
cd inhere
```
6. Find files of a specific size (1033 bytes) and check which files are human-readable.
```bash
find . -type f -size 1033c -exec file {} +
```
7. View the content of the human-readable file.
```bash
cat .file2
````

Flag (Password)
```
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```