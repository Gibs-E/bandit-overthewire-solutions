# Bandit Level 09 ➔ Level 10

## 🧠 Goal:
The password for the next level is stored in the file **`data.txt`**, which has been encoded with **ROT13** cipher. You need to decode it to get the password.

---

## 🔐 Login:
```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

## 🧾 Password Found:
`<truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk`

## 📘 What I Learned:
- How to decode ROT13 using the tr (translate) command.
-	The basics of substitution ciphers.
-	That tr can quickly map one set of characters to another for transformations.
