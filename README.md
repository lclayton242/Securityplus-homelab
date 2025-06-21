# Security+ Homelab Portfolio

This repository is a hands-on portfolio built while preparing for the **CompTIA Security+ certification (SY0-701)**. It demonstrates practical cybersecurity skills across system hardening, vulnerability scanning, and firewall implementation using real tools in virtual environments.

![license](https://img.shields.io/badge/license-MIT-blue)
![status](https://img.shields.io/badge/build-passing-brightgreen)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Stage Breakdown](#stage-breakdown)
3. [Folder Structure](#folder-structure)
4. [Getting Started](#getting-started)
5. [Contributing](#contributing)

## Project Goals

- Build a realistic, local homelab in VirtualBox
- Apply layered security controls at OS and network levels
- Capture and commit proof-of-work as a public GitHub portfolio
- Reinforce concepts covered in the Security+ exam domains

## Stage Breakdown

| Stage | Description | Folder |
|-------|-------------|--------|
| 1️ VM Setup | Installed and configured Ubuntu Server | [`ubuntu-hardening`](./ubuntu-hardening) |
| 2️ Hardening | Enabled UFW, SSH config, and patching | [`bash-history.txt`](./ubuntu-hardening/bash-history.txt) |
| 3️ Scanning | Ran Nmap and captured output | [`nmap-report.txt`](./ubuntu-hardening/nmap-report.txt) |
| 4️ Firewall | Built pfSense firewall VM with SSH-only rule | [`pfsense-lan-rules.png`](./ubuntu-hardening/screenshots/pfsense-lan-rules.png) |
| 5️ Log Forwarding & Graylog | Graylog stack + syslog stream | `[`logging/`](logging/) |


## Live Proof-of-Work

All stages include:

- Screenshots of successful implementation
- Exported scan and configuration files
- GitHub commit history for traceability

## Tech Stack

- VirtualBox
- Ubuntu 24.04 LTS
- pfSense 2.8.0
- Nmap
- UFW (Uncomplicated Firewall)

## Upcoming Stages

- Stage 6: Threat detection in TryHackMe / BlueTeamLabs
- Final: Resume-ready PDF + GitHub Pages showcase

---

> Built by [Luke Clayton](https://github.com/lclayton242) as part of a 9-week Security+ sprint challenge.
