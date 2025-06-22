# Bandit Level 26 ➔ Level 27

## 🧠 Goal:
You have a **private SSH key** located in the home directory.  
Use it to SSH into `bandit27` — no password needed.

---

## 🔐 Login:
```bash
ssh bandit26@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cat sshkey.private
nano bandit26_key
# Paste the private key here
chmod 600 bandit26_key
ssh -i bandit26_key bandit27@bandit.labs.overthewire.org -p 2220
```

## 🧾 Password Found:
`3ba3118a22e93127a4ed485be72ef5ea`

## 📘 What I Learned:
- How to use a private key to authenticate with SSH.
-	Importance of securing private keys (chmod 600 is essential).
-	Another example of secure access bypassing passwords entirely.
