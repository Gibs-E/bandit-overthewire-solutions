# Bandit Level 19 ➔ Level 20

## 🧠 Goal:
The password for the next level is stored in a file **only accessible** by a setuid binary called `bandit20-do`.  
You must use this program to read the password file as the `bandit20` user.

---

## 🔐 Login:
```bash
ssh bandit19@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
./bandit20-do cat /etc/bandit_pass/bandit20
```

## 🧾 Password Found:
`GbKksEFF4yrVs6il55v6gwY5aVje5f0j`

## 📘 What I Learned:
- How setuid binaries allow you to run commands as another user.
-	How to pass a command as an argument to an executable.
-	The importance of file permissions and privilege escalation through controlled tools.
