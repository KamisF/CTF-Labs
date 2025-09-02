# Bandit - Level 2

## Objective
The goal of this level is to find the password for Level 3. The password for the next level is stored in a file called --spaces in this filename-- located in the home directory

## Steps
1. Open the terminal.
2. Connect to the server using SSH:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
3. Enter the password for level 1
4. List all files
```bash
ls -a
```
5. Locate the file named "--spaces in this filename--"
```bash
cat ./--spaces\in\this\filename--"
```
Flag (Password)
```
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```