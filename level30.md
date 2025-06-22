# Bandit Level 30 ➔ Level 31

## 🧠 Goal:
There's a binary file called `bandit31` in the home directory.  
This binary **expects an environment variable called `LEGEND` to be set** to the password from the previous level.

If it is set correctly, it will print the password for the next level.

---

## 🔐 Login:
```bash
ssh bandit30@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
LEGEND=b5Ycw5sTw7x9S7GkUD3fjwlhbEZHTBmw ./bandit31
```

## 🧾 Password Found:
`tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S`

## 📘 What I Learned:
- How environment variables can be required by binaries to control behavior.
- That password validation can be done through external variable checks.
-	How to temporarily export and use environment variables inline.
