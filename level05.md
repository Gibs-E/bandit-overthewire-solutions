# Bandit Level 05 ➔ Level 06

## 🧠 Goal:
The password for the next level is stored in a file in the **inhere** directory, which is:
- Human-readable
- 1033 bytes in size
- Not executable
- Not a directory

You need to identify and read that specific file.

---

## 🔐 Login:
```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cd inhere
ls -l
find . -type f -size 1033c ! -executable
cat ./-file07
```

## 🧾 Password Found:
`DXjZPULLxYr17uwoI01bNLQbtFemEgo7`

## 📘 What I Learned:
- How to use the find command to locate files by specific size and permissions.
-	What ! -executable means when filtering results.
-	How file attributes like size can be used to precisely identify targets.
