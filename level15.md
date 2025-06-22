# Bandit Level 15 ➔ Level 16

## 🧠 Goal:
The password for the next level is stored on the server. You must send the current password to **port 30001** on localhost **using SSL encryption**.

---

## 🔐 Login:
```bash
ssh bandit15@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
echo BfMYroe26WYalil77FoDi9qh59eK5xNr | openssl s_client -connect localhost:30001
```

## 🧾 Password Found:
`cluFn7wTiGryunymYOu4RcffSxQluehd`

## 📘 What I Learned:
- How to use openssl s_client to connect to a TCP port securely using SSL.
-	That not all netcat-like services are unencrypted — some require TLS/SSL.
-	Understanding the basics of secure communication over ports.
