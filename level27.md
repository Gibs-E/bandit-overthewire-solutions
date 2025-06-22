# Bandit Level 27 ➔ Level 28

## 🧠 Goal:
Inside the home directory, there is a **`bandit28`** executable.  
This program **creates a file named `/tmp/bandit28_*****`** with the password for the next level, but **only if run by bandit27**.

---

## 🔐 Login:
```bash
ssh bandit27@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
./bandit28
cat /tmp/bandit28_aBZ0W5EmUfAf7kHTQeOwd8bfvkuijFGY
```

## 🧾 Password Found:
`aBZ0W5EmUfAf7kHTQeOwd8bfvkuijFGY`

## 📘 What I Learned:
- How executables can securely write to temporary files.
-	The importance of checking file creation output to locate credentials.
-	That privilege-restricted programs often leave behind accessible data when used properly.
