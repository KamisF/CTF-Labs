# Bandit - Level 3

## Objective
The goal of this level is to find the password for Level 4. The password is stored in a hidden file in the home directory.

## Steps
1. Open the terminal.
2. Connect to the server using SSH:

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```
3. Enter the password for level 2
4. List all files list files including hidden ones (ls -a), locate the hidden file, and read its content using commands like cat, less, or more to find the password for the next level.
```bash
ls -a
```
5. Locate the Directory named inhere.
```bash
cd inhere
```
6. List all files again with ls -a and open the hidden file.
```bash
ls -al
total 12
drwxr-xr-x 2 root    root    4096 Aug 15 13:16 .
drwxr-xr-x 3 root    root    4096 Aug 15 13:16 ..
-rw-r----- 1 bandit4 bandit3   33 Aug 15 13:16 ...Hiding-From-You
bandit3@bandit:~/inhere$ cat ...Hiding-From-You 
````

Flag (Password)
```
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```