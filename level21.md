# Bandit Level 21 ➔ Level 22

## 🧠 Goal:
A program named `cronjob_bandit22.sh` is being run every minute by a cron job under the user `bandit22`.  
You need to read the script, understand what it does, and find where it saves the password.

---

## 🔐 Login:
```bash
ssh bandit21@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cd /etc/cron.d/
cat cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/$(cat /etc/bandit_pass/bandit21)
cat /tmp/gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
```

## 🧾 Password Found:
`Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI`

## 📘 What I Learned:
- How to inspect and analyze cron job files in /etc/cron.d.
-	How to trace shell scripts to follow where outputs are written.
-	Using password files from one level to unlock the next securely.
