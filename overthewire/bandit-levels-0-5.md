# OverTheWire Bandit – Levels 0 to 5

These are my personal notes and solutions for OverTheWire’s Bandit levels 0 to 5. Bandit is designed to teach basic Linux commands and terminal navigation for beginners.

---

## 🔹 Level 0 → Level 1

### 🎯 Goal:
Log in to the server using SSH.

### 🔑 Solution:
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
# Password: bandit0
```
💡 What I Learned:

    How to connect to a remote machine using SSH

    The use of a non-standard port (2220)

## 🔹 Level 1 → Level 2

🎯 Goal:
Find a file called readme in the home directory and display its contents.

🔑 Solution:
```bash
    ls
    cat readme
```
💡 What I Learned:

Basic file listing with ls

Reading file content using cat

## 🔹 Level 2 → Level 3

🎯 Goal:

Find a file with a space in the filename.

🔑 Solution:
```bash
    ls
    cat "spaces in this filename"
```
💡 What I Learned:
How to handle filenames with spaces using quotes

## 🔹 Level 3 → Level 4

🎯 Goal:
Find a hidden file in the home directory.

🔑 Solution:
```bash
    ls -a
    cat .hidden
```
💡 What I Learned: 
Hidden files start with a . and are shown with ls -a

## 🔹 Level 4 → Level 5

🎯 Goal:
Find the human-readable file in a folder full of random data files.

🔑 Solution:
```bash
    cd inhere
    file *
    # Look for the one that says 'ASCII text'
    cat <filename>
```
💡 What I Learned:
The file command tells you the type of content in each file

How to identify human-readable data in a noisy folder

✅ Summary of What I’ve Learned So Far:

SSH basics

File navigation and viewing

Handling tricky filenames

Detecting hidden files

Identifying readable content with file




