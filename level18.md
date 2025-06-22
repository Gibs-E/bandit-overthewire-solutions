# Bandit Level 18 ➔ Level 19

## 🧠 Goal:
The password for the next level is stored **in the password file**, but **you cannot log out** after logging in — the shell immediately logs you out.  
You’ll need to use a **non-interactive shell** command to read the password file in one step.

---

## 🔐 Login:
```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat /etc/bandit_pass/bandit18"
```

## 🧾 Password Found:
`IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x`

## 📘 What I Learned:
- How to run a single remote command using SSH non-interactively.
-	That some user environments may be restricted or immediately closed.
-	How to work around login limitations in Linux with inline command execution.
