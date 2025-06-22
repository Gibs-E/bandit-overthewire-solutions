# Bandit Level 08 ➔ Level 09

## 🧠 Goal:
The password for the next level is stored in the file **`data.txt`**, which contains base64-encoded text. You need to decode it to find the password.

---

## 🔐 Login:
```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cat data.txt | base64 --decode
```

## 🧾 Password Found:
`UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR`

## 📘 What I Learned:
- How to decode base64-encoded strings using base64 --decode.
- How to pipe file content into a decoding command for quick analysis.
