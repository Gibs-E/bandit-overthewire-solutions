# Bandit Level 20 ➔ Level 21

## 🧠 Goal:
There's a program listening on **localhost:22220** that only sends the password if it receives the correct input.  
You need to:
1. Use the setuid binary `suconnect` to connect to that port.
2. Provide the current password.

---

## 🔐 Login:
```bash
ssh bandit20@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
./suconnect 21
```

## 🧾 Password Found:
`gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr`

## 📘 What I Learned:
- How to interact with setuid programs that manage socket-based communication.
-	That some level transitions require scripted or privileged utilities to interact with network ports.
-	The importance of matching input/output expectations when sending data to services.
