# Bandit Level 22 ➔ Level 23

## 🧠 Goal:
There’s a **cron job** running a script as `bandit23`, located in `/usr/bin/cronjob_bandit23.sh`.  
Your task is to exploit this job to make it output the password for bandit23 somewhere you can access it.

---

## 🔐 Login:
```bash
ssh bandit22@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cat /usr/bin/cronjob_bandit23.sh
cd /tmp/bandit22
ls
cat password
```

## 🧾 Password Found:
`jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n`

## 📘 What I Learned:
- How to use scheduled cron jobs to indirectly access restricted data.
-	That some scripts use user-based temp folders (/tmp/$(whoami)) to isolate output.
-	How persistence (waiting 1 minute) pays off in time-based automation.
