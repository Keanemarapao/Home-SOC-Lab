# Home SOC Lab

A complete Security Operations Center (SOC) lab built using Windows Server, Windows 11, Kali Linux, Active Directory, Sysmon, and Splunk Enterprise.

## Objective

Simulate real-world cyber attacks in a Windows Active Directory environment and investigate security events using Splunk SIEM.

---

## Technologies

- Windows Server 2022
- Windows 11
- Kali Linux
- Active Directory
- Splunk Enterprise
- Sysmon
- PowerShell
- VirtualBox

---

## Architecture

Kali Linux
↓

Windows 11 Client
↓

Windows Server (Domain Controller)

↓

Splunk Enterprise

↓

Sysmon Event Logs

---

## Lab Features

- Active Directory Domain
- Centralized Windows Logging
- Sysmon Telemetry
- PowerShell Monitoring
- Authentication Monitoring
- Network Event Logging
- Detection Rules
- Incident Investigation

---

## Simulated Attacks

- Password Spray
- Brute Force Login
- Nmap Scan
- PowerShell Download Cradle
- Mimikatz Execution
- Reverse Shell
- Scheduled Task Persistence

---

## Detection Examples

### Failed Login Detection

```spl
index=wineventlog EventCode=4625
| stats count by Account_Name, Workstation_Name
```

### Successful Logins

```spl
index=wineventlog EventCode=4624
```

### PowerShell Execution

```spl
index=sysmon EventCode=1 Image="*powershell.exe"
```

### Network Connections

```spl
index=sysmon EventCode=3
```

### Process Creation

```spl
index=sysmon EventCode=1
```

---

## Incident Reports

Each attack includes:

- Timeline
- MITRE ATT&CK Mapping
- IOC
- Detection Query
- Screenshots
- Findings
- Remediation

---

## Skills Demonstrated

- SIEM
- Windows Logging
- Detection Engineering
- Incident Response
- Active Directory Administration
- Threat Hunting
- Splunk SPL
- Sysmon Analysis
