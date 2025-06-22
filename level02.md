# Bandit Level 02 ➔ Level 03

## 🧠 Goal:
_The password for the next level is stored in a file called `spaces in this filename` located in the home directory._

## 🔐 Login:
```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ls
cat "spaces in this filename"
```

## 🧾 Password Found:
`UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`

## 📘 What I Learned:
- How to handle file names with spaces using quotes or escape characters (`\`).
- More practice navigating and working in the Linux file system.
