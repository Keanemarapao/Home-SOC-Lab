# 🛡️ SOC Analyst Home Lab

> A complete Security Operations Center (SOC) home lab built in VirtualBox to simulate a real enterprise environment. This project focuses on log collection, network monitoring, intrusion detection, threat hunting, incident response, and security operations using industry-standard open-source tools.

---

## 📌 Project Overview

The purpose of this lab is to gain hands-on experience with technologies commonly used by SOC Analysts in enterprise environments.

Throughout this project I will build a multi-machine virtual environment, configure centralized logging, detect malicious activity, investigate security incidents, and document findings as if working in a real Security Operations Center.

---

## 🎯 Objectives

- Build an enterprise-style virtual network
- Configure secure Linux and Windows endpoints
- Deploy a centralized monitoring platform
- Collect and analyze logs
- Detect network and host-based attacks
- Perform threat hunting
- Conduct incident response investigations
- Build a professional cybersecurity portfolio

---

# 🖥️ Lab Architecture

```
                           Internet
                               │
                          VirtualBox NAT
                               │
                    ┌────────────────────┐
                    │  Ubuntu Server     │
                    │  SOC Infrastructure│
                    └────────────────────┘
                      │              │
        ┌─────────────┘              └─────────────┐
        │                                          │
 ┌───────────────┐                      ┌────────────────┐
 │ Windows 10    │                      │ Ubuntu Desktop │
 │ Corporate PC  │                      │ Linux Endpoint │
 └───────────────┘                      └────────────────┘
```

---

# 🖥️ Virtual Machines

## Ubuntu Server 22.04

Role:

- SOC Infrastructure
- SIEM
- Network Monitoring
- Threat Intelligence

Services to be deployed:

- Wazuh
- ELK Stack
- Zeek
- Suricata
- MISP

---

## Windows 10

Role:

- Corporate workstation
- Endpoint monitoring
- Attack simulation
- Sysmon logging

---

## Ubuntu Desktop

Role:

- Linux endpoint
- Security testing
- Network analysis
- Threat hunting workstation

---

# 🌐 Network Design

## Management Network

```
192.168.56.0/24
```

Used for:

- SSH
- Administration
- SIEM Management
- Dashboard Access

---

## Internal Monitored Network

```
10.0.0.0/24
```

Used for:

- Endpoint communication
- Network monitoring
- Attack simulations
- IDS visibility

---

## NAT Network

Provides:

- Internet access
- Package downloads
- Threat intelligence updates

---

# 🛠️ Technologies

## Virtualization

- VirtualBox

## Operating Systems

- Ubuntu Server 22.04
- Ubuntu Desktop 22.04
- Windows 10

## Security Tools

- Wazuh
- Elasticsearch
- Kibana
- Logstash
- Zeek
- Suricata
- MISP
- Sysmon
- Sigma Rules

## Networking

- Wireshark
- TCP/IP
- SSH
- DNS
- DHCP

## Offensive Security

- Kali Linux (future)
- Nmap
- Hydra
- Metasploit

---

# 📚 Learning Roadmap

## Phase 1

- VirtualBox Setup
- Network Configuration
- Ubuntu Server
- Windows 10
- Ubuntu Desktop

---

## Phase 2

- System Hardening
- SSH Configuration
- Firewall Configuration
- User Management

---

## Phase 3

- Wazuh Installation
- Agent Deployment
- Dashboard Configuration

---

## Phase 4

- Zeek Installation
- Network Monitoring
- Traffic Analysis

---

## Phase 5

- Suricata
- IDS Rules
- Alert Generation

---

## Phase 6

- Threat Hunting
- Log Analysis
- Detection Engineering

---

## Phase 7

- ELK Stack
- Dashboards
- Visualization

---

## Phase 8

- Incident Response
- IOC Analysis
- Malware Investigation

---

# 🔍 Skills Demonstrated

- Linux Administration
- Windows Administration
- Virtualization
- Network Security
- Log Analysis
- SIEM Administration
- Endpoint Monitoring
- Threat Hunting
- Incident Response
- Detection Engineering
- Security Monitoring
- IDS/IPS Management
- Firewall Configuration

---

# 📈 MITRE ATT&CK Coverage

Examples include:

- Initial Access
- Discovery
- Credential Access
- Persistence
- Defense Evasion
- Command and Control
- Exfiltration

Each attack simulation will be mapped to its corresponding MITRE ATT&CK techniques.

---

# 📸 Project Progress

## Week 1

- [ ] VirtualBox Installation
- [ ] Create Virtual Networks
- [ ] Ubuntu Server Installation
- [ ] Windows Installation
- [ ] Ubuntu Desktop Installation

---

## Week 2

- [ ] Secure SSH
- [ ] Configure Firewall
- [ ] Install Monitoring Agents

---

## Week 3

- [ ] Install Wazuh
- [ ] Deploy Agents
- [ ] Verify Log Collection

---

## Week 4

- [ ] Install Zeek
- [ ] Analyze Network Traffic

---

## Week 5

- [ ] Install Suricata
- [ ] Generate IDS Alerts

---

## Week 6

- [ ] Threat Hunting Exercises
- [ ] Detection Rules

---

## Week 7

- [ ] Deploy ELK Stack
- [ ] Create Dashboards

---

## Week 8

- [ ] Incident Response Report
- [ ] Portfolio Documentation

---

# 📷 Screenshots

This repository will include screenshots for:

- VirtualBox Configuration
- Network Layout
- Wazuh Dashboard
- Kibana Dashboards
- Zeek Logs
- Suricata Alerts
- Threat Hunting Queries
- Incident Response Reports

---

# 💻 Hardware Configuration

## Minimum (8GB RAM)

Suitable for completing the lab with limited performance.

- Ubuntu Server — 3 GB RAM
- Windows 10 — 2 GB RAM
- Ubuntu Desktop — 2 GB RAM

---

## Recommended (16GB RAM)

Best balance of performance and resource usage.

- Ubuntu Server — 6 GB RAM
- Windows 10 — 4 GB RAM
- Ubuntu Desktop — 4 GB RAM

---

## Instructor Configuration (32GB RAM)

Matches the original course setup.

- Ubuntu Server — 8 GB RAM
- Windows 10 — 4 GB RAM
- Ubuntu Desktop — 4 GB RAM

---

# 🎓 Goal

By the end of this project I will have built a fully functional SOC lab capable of:

- Centralized log collection
- Network traffic monitoring
- Intrusion detection
- Threat hunting
- Endpoint monitoring
- Incident response
- Security investigations

This project is intended to demonstrate practical SOC Analyst skills that align with entry-level cybersecurity and Security Operations Center roles.
