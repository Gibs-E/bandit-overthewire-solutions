# Bandit Level 10 ➔ Level 11

## 🧠 Goal:
The password for the next level is stored in the file **`data.txt`**, which contains binary data. You need to extract only the human-readable text from it.

---

## 🔐 Login:
```bash
ssh bandit10@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
strings data.txt
```

## 🧾 Password Found:
`IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`

## 📘 What I Learned:
- How to use strings to extract printable characters from a binary file.
-	How to visually identify passwords in noisy data.
-	Why tools like strings are useful for analyzing non-text files.
