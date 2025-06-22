# Bandit Level 07 ➔ Level 08

## 🧠 Goal:
The password for the next level is stored in the file **`data.txt`**, which contains many lines. You need to find the **only line** that occurs **exactly once**.

---

## 🔐 Login:
```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cat data.txt | sort | uniq -u
```

## 🧾 Password Found:
`cvX2JJa4CFALtqS87jk27qwqGhBM9plV`

## 📘 What I Learned:
- How to use sort and uniq together to detect unique values in a file.
-	That command-line text processing is powerful for analyzing large datasets quickly.
-	Reinforced the use of pipes (|) to combine commands effectively.
