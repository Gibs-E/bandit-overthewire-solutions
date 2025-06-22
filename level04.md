# Bandit Level 04 → Level 05

## 🧠 Goal:
_The password for the next level is stored in a hidden file in the inhere directory. The file is human-readable, not a directory, not executable, and its name starts with a dot (.).
_

## 🔐 Login:
```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ls -a
cd inhere
ls -a
cat .hidden
```

## 🧾 Password Found:
`koReBOKuIDDepwhWk7jZC0RTdopnAYKh`

## 📘 What I Learned:
- How to view hidden files using ls -a.
-	How to identify non-executable, human-readable files.
-	Better understanding of how Linux treats filenames starting with a dot (.) as hidden.

