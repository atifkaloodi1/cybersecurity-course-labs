# 🧪 Lab 1: Nmap Scan Report

## 🎯 Objective
Perform network scanning using **Nmap** to identify open ports, running services, and operating system details of a target machine.

---

## 🛠️ Tools Used
- Nmap v7.93
- Kali Linux or any Linux distro
- Target: Metasploitable VM or vulnerable test machine

---

## 🧪 Commands Used
```bash
nmap -sS -T4 -v 192.168.1.100
nmap -sV -O 192.168.1.100


📊 Findings

| Port | Service | Version           | State |
| ---- | ------- | ----------------- | ----- |
| 22   | SSH     | OpenSSH 4.7       | Open  |
| 80   | HTTP    | Apache 2.2.8      | Open  |
| 139  | NetBIOS | Samba smbd 3.0.20 | Open  |


🔍 Observations
Apache web server on port 80 may expose default pages.

Samba service on port 139 could be vulnerable to remote exploits.

✅ Conclusion
This scan helped identify potentially exploitable services. In a real SOC environment, we would now check if patches are available or further vulnerability assessment is needed.


---
### 📁 `projects/resume_projects.md`

```markdown
# 🧾 Projects for Resume

This document outlines projects I completed as part of the Cybersecurity Analyst diploma at Willis College.

---

## 🛡️ SOC Home Lab
- Built a virtual home lab with firewall, IDS/IPS, and a SIEM (Splunk/Elastic).
- Collected and analyzed real-time logs from simulated attacks.
- Automated alerting for brute-force login attempts and suspicious network scans.

---

## 🔍 Network Scanning Automation
- Scripted daily scans using Nmap + Cron.
- Scheduled email notifications for open port changes.

---

## 🧪 Incident Response Simulation
- Responded to a mock phishing attack.
- Identified indicators of compromise and performed log correlation using Splunk.

---

**📌 Tech Stack:** Nmap, Splunk, Wireshark, Snort, Ubuntu Server, Bash, Windows 10, VirtualBox



