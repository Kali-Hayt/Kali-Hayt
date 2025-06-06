# 🖥️ HTB Machine — fawn

## 🧾 Info
- Release Date: 2021-06-05
- Difficulty: Very Easy
- IP Address: 10.129.16.89
- OS: Linux

---

## 📡 Enumeration

### Nmap
```bash
nmap -sC -sV -oN fawn-nmap.txt 10.129.16.89

Other scans / Notes:
FTP open on port 21

Anonymous login allowed (FTP code 230)

flag.txt found

⚔️ Exploitation
Initial Exploit: FTP anonymous file download

Shell Access: ❌ No shell on this box

Privilege Escalation: ❌ Not applicable

🧠 What I Learned
FTP enumeration with nmap

Importance of checking for anonymous access

FTP status codes like 230

🧪 Practice Areas
 FTP

 Web

 PrivEsc

 Shell Access

🔁 Work History
 2025-06-05: Scanned with nmap, downloaded flag.txt via FTP
