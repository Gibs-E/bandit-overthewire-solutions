# Bandit Level 11 ➔ Level 12

## 🧠 Goal:
The password for the next level is stored in the file **`data.txt`**, which is a **hexdump** of a binary file. You need to:
1. Recreate the original binary from the hexdump.
2. Extract the human-readable password from it.

---

## 🔐 Login:
```bash
ssh bandit11@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
xxd -r data.txt > restored_file
strings restored_file
```

## 🧾 Password Found:
`5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu`

## 📘 What I Learned:
- How to reverse a hexdump using xxd -r.
-	How to handle hex-encoded data and restore it to its original format.
-	Combining tools like xxd and strings to retrieve data from transformed files.
