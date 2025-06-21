# ✅ Stage 5 – Graylog Working with Syslog Forwarding

**Date Completed:** 2025-06-20  
**Author:** Luke Clayton  
**Repo:** homelab

---

## 🎯 Goal

To successfully forward system logs from the Ubuntu-Homelab VM to a Graylog server using `rsyslog` over UDP and organize the logs into a stream.

---

## 🧩 What Was Completed

- ✅ Graylog installed via Docker Compose
- ✅ Web GUI accessible at `http://10.0.0.163:9000`
- ✅ Syslog UDP input created on port `12201`
- ✅ Homelab VM forwarding logs using rsyslog
- ✅ Logs visible in Graylog search
- ✅ Created stream: `Homelab Syslog Stream`
- ✅ Stream confirmed working by filtering messages by source: `homelab`
- ✅ Manual test log appeared using `logger` command

---

## 🛠 Config Files Included

- [`graylog/docker-compose.yml`](../graylog/docker-compose.yml)
- [`rsyslog/90-graylog.conf`](../rsyslog/90-graylog.conf)

---

## 💾 Snapshot Saved

VirtualBox snapshot name:
