# SOC Home Lab | Active Directory + Splunk + Azure

## Overview

This project documents my cybersecurity home lab designed to build hands-on skills in:

- Active Directory administration
- Security Information and Event Management (SIEM)
- Threat detection
- Log analysis
- Incident response
- Vulnerability management
- Cloud identity security

The goal is to create a realistic SOC-style environment for learning and expanding cybersecurity skills.

---

## Lab Architecture

Internet

↓

Router/NAT

↓

Windows Server 2019 Domain Controller

↓

Windows Client Machine

↓

Splunk SIEM

↓

Sysmon Logging

↓

Kali Linux Attack Machine

↓

Azure/Entra ID Integration

---

## Technologies Used

### Operating Systems

- Windows Server 2019
- Windows 10
- Kali Linux

### Security Tools

- Splunk Enterprise
- Splunk Universal Forwarder
- Sysmon
- Nessus Essentials

### Cloud

- Azure
- Entra ID

### Virtualization

- VirtualBox

---

## Project Goals

- Build Active Directory environment
- Create users, groups, and Organizational Units
- Configure Group Policy Objects
- Forward security logs into Splunk
- Create dashboards and alerts
- Simulate attacks
- Investigate incidents
- Map attacks to MITRE ATT&CK
- Document findings

---

## Skills Demonstrated

- Identity and Access Management
- Active Directory Administration
- Threat Hunting
- Incident Response
- SIEM Analysis
- Windows Event Analysis
- Log Correlation
- Security Monitoring

---

## Sample SPL Queries

### Failed Logins

```spl
index=wineventlog EventCode=4625
```

### Successful Logins

```spl
index=wineventlog EventCode=4624
```

### New User Creation

```spl
index=wineventlog EventCode=4720
```

### Account Lockouts

```spl
index=wineventlog EventCode=4740
```

---

## Future Expansion

- Honeypot deployment
- Heat map dashboards
- Azure Sentinel
- Threat hunting playbooks
- SOAR concepts

