# Bandit - Level 1

## Objective
The goal of this level is to log into the Bandit server via SSH using the provided credentials and find the password for the next level.

## Steps
1. Open the terminal.
2. Connect to the server using SSH:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
3. Enter the password for Level 1
```bash
bandit0
```
4. List the files in the home Directory to find the next password
```bash
ls 
```
5. Read the file containing the password
```bash
cat readme
```
Flag (Password)
```
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```