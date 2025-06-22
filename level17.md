# Bandit Level 17 ➔ Level 18

## 🧠 Goal:
There are **two files** in `/etc/bandit_pass`:
- One belongs to **bandit17** (your user)
- The other belongs to **bandit18**

Your task is to find the one **that is readable by your user (bandit17)** but **not owned by bandit17** — and get the password from it.

---

## 🔐 Login:
```bash
ssh bandit17@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
ls -l /etc/bandit_pass/
# Identify which file is *not* owned by bandit17 but still readable
cat /etc/bandit_pass/bandit18
```

## 🧾 Password Found:
`kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd`

## 📘 What I Learned:
- How to interpret file permissions and ownership using ls -l.
-	That you can read files not owned by you if the permissions allow it.
-	More practice navigating and analyzing file metadata on Linux systems.
