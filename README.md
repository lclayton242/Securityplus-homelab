# Ubuntu Hardening Proof — Security+ Lab

This folder documents the hardening of a baseline Ubuntu Server 22.04 virtual machine as part of Security+ (SY0-701) hands-on study.

## What was hardened

- Enabled UFW firewall
- Installed system updates (`sudo apt update && sudo apt upgrade -y`)
- Created a non-root sudo user (`luke`)
- Installed Guest Additions for VirtualBox
- Secured clipboard, mount access, and reboot process

## Screenshots

![Ubuntu Login Prompt](screenshots/login.png)

## Command Log

See [`bash-history.txt`](bash-history.txt) for a full exported log of all commands executed during setup.

---

> **Connect with me:**  
> [LinkedIn](www.linkedin.com/in/lukeaclayton)
