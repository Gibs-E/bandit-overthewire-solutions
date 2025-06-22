# Bandit Level 25 ➔ Level 26

## 🧠 Goal:
There's a **setuid binary** called `bandit26` in the home directory.  
When executed, it **connects to localhost on port 30001** and sends the current password.  
You must **intercept the connection** to retrieve the next password.

---

## 🔐 Login:
```bash
ssh bandit25@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
mkdir /tmp/mylistener
cd /tmp/mylistener
nc -l -p 30001 > output.txt &
~/bandit26
cat output.txt
```

## 🧾 Password Found:
`5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z`

## 📘 What I Learned:
- How to intercept connections using nc -l -p.
-	That local binaries can leak information through insecure network usage.
-	How setuid programs behave and why network eavesdropping matters even on localhost.
