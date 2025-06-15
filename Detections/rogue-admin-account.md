# 🔐 Detection: Rogue Administrator Account Creation

---

## 🧭 Description

This detection identifies the creation of a new local user and the elevation of that user to the **Administrators** group — a common persistence tactic used by attackers after initial access or privilege escalation.

---

## 📌 MITRE ATT&CK Mapping

| Technique | ID |
|----------|----|
| Account Manipulation | T1098 |
| Create Account | T1136.001 |
| Permission Groups Discovery | T1069.001 |

---

## 🧪 Lab Simulation
![Elevated Command Prompt](https://raw.githubusercontent.com/Dabruzzinator/Wazuh-Sysmon-Lab/main/screenshots/elevated-command-prompt.jpg)
A rogue local admin account was created using the following commands:

```cmd
net user badactor Sup3rSecure! /add
![Bad Actor Created](https://raw.githubusercontent.com/Dabruzzinator/Wazuh-Sysmon-Lab/main/screenshots/Badactor%20creation.JPG)
net localgroup administrators badactor /add


