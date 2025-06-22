# Bandit Level 16 ➔ Level 17

## 🧠 Goal:
The password for the next level can be retrieved by submitting the current password to a **custom service** running on **port 31000**.  
However, the port is protected by **port knocking** — a sequence of ports must be accessed first in the correct order.

---

## 🔐 Login:
```bash
ssh bandit16@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
nmap -p- -sV --script=ssh-hostkey localhost
for port in 31790 31960 31790; do nc -zv localhost $port; done
nc localhost 31000
```

## 🧾 Password Found:
`xbgTi9NZZBrVRn5aPyU4q6537eVjdV3g`

## 📘 What I Learned:
- How port knocking can be used as a security measure to temporarily open ports.
-	How to simulate knocking using nc -zv in sequence.
-	That advanced services may require extra steps just to become accessible.
