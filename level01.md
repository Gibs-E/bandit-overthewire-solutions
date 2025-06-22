# Bandit Level 01 ➔ Level 02

## 🧠 Goal:
_The password for the next level is stored in a file called `-`, located in the home directory._

## 🔐 Login:
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ls
cat ./-
```

## 🧾 Password Found:
`CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`

## 📘 What I Learned:
•	How to read a file with a tricky name (a dash -) using relative path (./-).
•	The importance of escaping or handling special characters in file names.
