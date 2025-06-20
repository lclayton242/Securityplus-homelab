# Ubuntu Hardening Lab (Security+ Portfolio Project)

This repository showcases a fully documented cybersecurity lab used to prepare for the CompTIA Security+ certification. It demonstrates hands-on skills in VM setup, system hardening, vulnerability scanning, and firewall configuration using industry-standard tools like Ubuntu, Nmap, and pfSense.

---

## Lab Summary
**Goal:** Simulate a secure internal network environment and apply layered security practices across OS and firewall levels.

**Tools Used:**
- VirtualBox
- Ubuntu Server 24.04 LTS
- pfSense Firewall (2.8.0)
- Nmap

**Proof-of-Work:** All actions are logged, screenshotted, and committed to GitHub.

---

## Stage 1 – VM Setup
- Installed Ubuntu 24.04 LTS Server on VirtualBox
- Created a non-root user (`luke`)
- Enabled OpenSSH for remote administration

![pfSense Rules](screenshots/login.png) — Ubuntu shell access confirmation

---

## Stage 2 – System Hardening
- Ran full system update: `sudo apt update && sudo apt upgrade`
- Enabled and configured UFW firewall
- Verified SSH config and user permissions
- Exported bash history to track all secure system changes

📄 [`bash-history.txt`](ubuntu-hardening/bash-history.txt)

---

## Stage 3 – Vulnerability Scanning
- Installed `nmap`
- Scanned localhost (`127.0.0.1`) for open ports/services
- Captured and committed raw output

📄 [`nmap-report.txt`](ubuntu-hardening/nmap-report.txt)

---

## Stage 4 – Firewall Lab (pfSense)
- Created a new pfSense VM and connected it to an internal VirtualBox network
- Assigned dual interfaces (NAT = WAN, Internal = LAN)
- Cloned Ubuntu VM to act as LAN client
- Installed Ubuntu Desktop GUI to access pfSense via Firefox
- Logged in to pfSense admin panel
- Configured LAN rule to **only allow SSH (port 22)**
- Disabled default allow-all rule to enforce policy

📸 [`pfsense-lan-rules.png`](ubuntu-hardening/screenshots/pfsense-lan-rules.png)

---

## Next Stages (Planned)
- Stage 5: Log forwarding with Rsyslog + Graylog
- Stage 6: Simulated phishing detection in TryHackMe

---

## Repo File Tree (Key Files)
```bash
ubuntu-hardening/
├── bash-history.txt              # All shell commands run during hardening
├── nmap-report.txt              # Raw Nmap scan results
└── screenshots/
    ├── login.png                # Ubuntu shell login
    └── pfsense-lan-rules.png   # Final firewall rule config
