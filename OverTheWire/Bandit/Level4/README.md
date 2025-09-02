# Bandit - Level 4

## Objective
The goal of this level is to find the password for Level 5. The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Steps
1. Open the terminal.
2. Connect to the server using SSH:

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```
3. Enter the password for level 3
4. List all files list files including hidden ones (ls -a), locate the hidden file, and read its content using commands like cat, less, or more to find the password for the next level.
```bash
ls -a
```
5. Locate the Directory named inhere.
```bash
cd inhere
```
6. List all files in the directory to identify which file is human-readable:.
```bash
bandit4@bandit:~/inhere$ file ./*
./-file00: Non-ISO extended-ASCII text, with no line terminators, with overstriking
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
```
7. Read the human-readable file to get the password for the next level:
```bash
cat ./-file07
```

Flag (Password)
```
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```