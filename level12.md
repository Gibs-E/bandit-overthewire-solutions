# Bandit Level 12 ➔ Level 13

## 🧠 Goal:
The password for the next level is stored in the file **`data.txt`**, but it has been **compressed multiple times** with various compression formats. You need to **extract the password by reversing all the compression layers**.

---

## 🔐 Login:
```bash
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
mkdir temp
cp data.txt temp/
cd temp
xxd -r data.txt > data.bin
file data.bin
# Based on file type, run appropriate decompression steps:
# Example sequence:
zcat data.bin > layer1
bzip2 -d layer1
tar -xvf layer1.out
# Repeat until you reach plain text
```

## 🧾 Password Found:
`8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL`

## 📘 What I Learned:
- How to identify and handle multiple compression types using file.
-	How to systematically decompress nested files.
-	Importance of creating a safe workspace (mkdir temp) to avoid overwriting files.
