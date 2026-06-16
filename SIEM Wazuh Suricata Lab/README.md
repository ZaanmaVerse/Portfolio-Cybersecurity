# 🛡️ Integrated Intrusion Detection System (HIDS + NIDS)

## Overview

This project demonstrates the implementation of an integrated cybersecurity monitoring environment using **Wazuh (HIDS)** and **Suricata (NIDS)** to detect, monitor, and respond to host-based and network-based security threats in real time.

The system was designed to simulate a Security Operations Center (SOC) environment capable of identifying common attack techniques such as:

- Brute Force Attacks
- Port Scanning
- Vulnerability Scanning
- Web Shell Upload & Execution

---

## Business Value

Organizations often struggle to gain visibility into security events occurring across endpoints and network infrastructure.

This project provides:

✅ Real-time threat monitoring

✅ Centralized security event visibility

✅ Early detection of malicious activities

✅ Faster incident response capability

✅ Low-cost implementation using open-source technologies

---

## Architecture

```text
┌────────────────────┐
│ Kali Linux Attacker│
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Ubuntu Server      │
│ Wazuh Manager      │
│ Suricata NIDS      │
│ Email Alert System │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Windows Endpoint   │
│ Wazuh Agent        │
│ Apache Web Server  │
└────────────────────┘
```

---

## Technologies Used

### Security Monitoring

- Wazuh SIEM
- Suricata IDS
- Wazuh Agent

### Operating Systems

- Ubuntu Server
- Windows 11
- Kali Linux

### Security Testing

- Hydra
- Nmap
- Nikto

### Notification

- Postfix Mail Server

---

## Detection Use Cases

### 1. Brute Force Detection

**Scenario**

An attacker attempts multiple login requests using Hydra.

**Detection Logic**

- Monitor authentication failures
- Correlate repeated login failures
- Trigger alert after threshold exceeded

**Outcome**

- High severity alert generated
- Email notification sent to administrator

---

### 2. Port Scan Detection

**Scenario**

An attacker performs reconnaissance using Nmap.

**Detection Logic**

- Suricata detects scanning behavior
- Wazuh correlates Suricata events
- High-level alert generated

**Outcome**

- Scan activity identified in real time
- Security alert forwarded to SOC dashboard

---

### 3. Vulnerability Scan Detection

**Scenario**

Nikto performs web application reconnaissance.

**Detection Logic**

- Suricata detects vulnerability scanning signatures
- Custom correlation rule triggers high-priority event

**Outcome**

- Vulnerability assessment activity identified
- Email alert generated

---

### 4. Web Shell Detection

**Scenario**

A malicious PHP web shell is uploaded and executed.

**Detection Logic**

- Apache access logs monitored
- Wazuh custom rule detects shell execution patterns

**Outcome**

- Shell execution detected
- Security event escalated immediately

---

## Security Controls Implemented

| Control | Purpose |
|----------|----------|
| Wazuh HIDS | Host monitoring |
| Suricata NIDS | Network monitoring |
| Custom Rules | Threat correlation |
| Email Alerting | Incident notification |
| Log Collection | Centralized visibility |

---

## Key Results

| Attack Simulation | Detection Status |
|-------------------|------------------|
| Hydra Brute Force | ✅ Detected |
| Nmap Scan | ✅ Detected |
| Nikto Scan | ✅ Detected |
| Web Shell Upload | ✅ Detected |
| Web Shell Execution | ✅ Detected |

---

## Skills Demonstrated

### Security Operations (SOC)

- Security Monitoring
- Log Analysis
- Threat Detection
- Incident Identification
- Alert Triage

### Blue Team

- SIEM Administration
- IDS Configuration
- Detection Engineering
- Threat Hunting Fundamentals

### Infrastructure

- Linux Administration
- Windows Security Monitoring
- Network Security Monitoring

---

## Lessons Learned

Through this project, I gained hands-on experience in:

- Building a practical SOC laboratory
- Developing custom detection rules
- Integrating HIDS and NIDS technologies
- Investigating security events
- Understanding attacker behaviors and indicators

---

## Future Improvements

- Implement Active Response for automatic blocking
- Integrate threat intelligence feeds
- Add MITRE ATT&CK mapping
- Deploy dashboard reporting
- Build automated incident response workflows

---

## Project Status

✅ Completed

---

## Author

**Zaidan Mahfudz Azzam Saidi**

Cybersecurity Student | SOC Analyst Enthusiast | Blue Team
