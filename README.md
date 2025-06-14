# 🛡️ Wazuh + Sysmon Threat Detection Lab

This project is part of my hands-on security analyst training. It simulates real-world endpoint attacks, detects them using Sysmon and Wazuh, and showcases detection engineering, log analysis, and incident response techniques.

---

## 🎯 Goal

To demonstrate full-cycle detection from endpoint telemetry to SIEM alerting using free, open-source tools — built in a virtualized home lab for cybersecurity analyst career readiness.

---

## 🧠 Tools Used

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| **Sysmon**      | Endpoint telemetry (process, net, registry) |
| **Wazuh Agent** | Forward logs to SIEM             |
| **Wazuh Manager** | SIEM + Rule Engine              |
| **Kibana**      | Search and visualization         |
| **VirtualBox**  | Host lab (Windows 10 + Kali)     |

---

## 🧪 Simulated Attacks & Detections

| Attack # | Technique                  | Detection Outcome |
|----------|----------------------------|-------------------|
| 1        | PowerShell Scheduled Task (Persistence) | ✅ Detected in Wazuh |
| 2        | *(coming soon)* Rogue user creation     | 🔜                 |
| 3        | *(coming soon)* Registry backdoor       | 🔜                 |

See [`/detections`](./detections) for rule files and analysis.

---

## 📸 Screenshots

- Sysmon event logs captured in Wazuh
- Detected command line activity (calc.exe, schtasks)
- Custom filters in Kibana
- [Click here to view screenshots](./screenshots)

---

## 🧰 Config Files

- [`sysmonconfig-export.xml`](./configs/sysmonconfig-export.xml)
- [`ossec.conf`](./configs/ossec.conf)

---

## 🧾 Lab Setup Guide

Coming soon — I will share how I built the lab from scratch so others can replicate it.

---

## 📌 About Me

I'm transitioning from 4+ years in IT Help Desk with Security+, A+, Network+, and Google Cybersecurity certifications. This lab demonstrates my hands-on readiness for a Security Analyst role.

[Connect on LinkedIn](https://www.linkedin.com/) | [More Projects](https://github.com/yourusername)

Initial README build for lab
