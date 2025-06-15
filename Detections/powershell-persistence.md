# 🛠️ Detection: PowerShell Scheduled Task (Persistence Technique)

---

## 🔍 Description

This simulation demonstrates how adversaries can establish **persistence** on a Windows system using **PowerShell** to create a scheduled task that runs malicious code after reboot or at timed intervals. This is mapped to:

- **MITRE ATT&CK Technique T1053.005**: Scheduled Task / Job — Windows Task Scheduler

---

## 🎯 Goal of the Attack

To simulate a threat actor adding persistence to a compromised host using:

```powershell
powershell -NoP -NonI -W Hidden -Command "Start-Process calc.exe -WindowStyle Hidden"
Microsoft-Windows-Sysmon/Operational
data.win.system.event_id: 1
data.win.eventdata.commandLine: "*calc.exe*"
