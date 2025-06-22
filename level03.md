# Bandit Level 03 ➔ Level 04

## 🧠 Goal:
_The password for the next level is stored in a hidden file in the inhere directory._

## 🔐 Login:
```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ls
ls -a
cd inhere
cat .hidden
```

## 🧾 Password Found:
`pIwrPrtPN36QITSp3EQaw936yaFoFgAB`

## 📘 What I Learned:
- How to view hidden files using the -a flag with ls
- That files or directories starting with a . are hidden by default in Linux
-	Practiced changing directories and reading file contents
