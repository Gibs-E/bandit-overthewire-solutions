# Bandit Level 06 ➔ Level 07

## 🧠 Goal:
The password for the next level is stored in a file called `bandit7`, located in the **`/`** (root) directory. The file is **owned by user `bandit7`**, **group `bandit6`**, and **is 33 bytes in size**.

You need to use `find` to locate the file that matches all three conditions.

---

## 🔐 Login:
```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /<full/path/to/file>
```

## 🧾 Password Found:
`HKBPTKQnIay4Fw76bEy8PVxKZD7tfaru`

## 📘 What I Learned:
- How to search the entire filesystem with find.
-	Filtering by file size (-size 33c), owner (-user), and group (-group).
-	How to suppress permission errors using 2>/dev/null.
