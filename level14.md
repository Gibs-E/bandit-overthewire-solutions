# Bandit Level 14 ➔ Level 15

## 🧠 Goal:
The password for the next level is stored on the server, and you must send the current password to port **30000** on localhost using **netcat** (`nc`).

---

## 🔐 Login:
```bash
ssh bandit14@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
echo 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e | nc localhost 30000
```

## 🧾 Password Found:
`BfMYroe26WYalil77FoDi9qh59eK5xNr`

## 📘 What I Learned:
- How to send input through TCP using nc (netcat).
-	How local services can be used to retrieve sensitive information.
-	Simple client-server interaction using ports on the same machine.
