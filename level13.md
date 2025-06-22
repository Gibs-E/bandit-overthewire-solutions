# Bandit Level 13 ➔ Level 14

## 🧠 Goal:
The password for the next level is stored in the **`/etc/bandit_pass/bandit14`** file, but you are **not allowed to read it directly**.  
Instead, you must **log in to the next level using the current password via SSH** on localhost as `bandit14`.

---

## 🔐 Login:
```bash
ssh bandit13@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ssh bandit14@localhost -p 2220
# When prompted for password, use:
# 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
```

## 🧾 Password Found:
`4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`

## 📘 What I Learned:
- How to use SSH to connect to a local user account securely.
-	That file access restrictions can be bypassed through privilege chaining or lateral movement.
-	Understanding trust boundaries and why multi-user permissions matter in Linux.
