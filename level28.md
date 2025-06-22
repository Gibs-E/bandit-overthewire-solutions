# Bandit Level 28 ➔ Level 29

## 🧠 Goal:
There’s a **web service** running on port **25734**.  
To access the password for the next level, you need to send a **POST request** with a **secret key**.

The key is stored in the file:  
```bash
~/secret
```

## 🔐 Login:
```bash
ssh bandit28@bandit.labs.overthewire.org -p 2220
```

## 🛠️ Commands Used:
```bash
cat ~/secret
curl -X POST -d secret=jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt http://localhost:25734
```

## 🧾 Password Found:
`agvjfJzID7xBhMZwh0pZ0ccyiC`

## 📘 What I Learned:
- How to use curl to send POST requests.
-	That secrets or tokens can be used to authenticate access to restricted endpoints.
-	How web services can be accessed and interacted with locally from the command line.
