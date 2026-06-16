# Capture The Flag (CTF) Web Security Writeups

## Overview

This repository contains a collection of Web Security, Cryptography, Digital Forensics, and OSINT challenge writeups completed during the President University Capture The Flag (CTF) competition.

The purpose of this repository is to demonstrate practical cybersecurity skills including:

* Web Application Security Testing
* Vulnerability Identification
* Exploitation Methodology
* Security Impact Analysis
* Root Cause Analysis
* Secure Development Recommendations
* Technical Documentation

> All activities were conducted in a controlled Capture The Flag (CTF) environment for educational and ethical learning purposes.

---

## Objectives

This project was created to:

* Practice real-world cybersecurity problem solving
* Improve vulnerability assessment capabilities
* Strengthen web application security knowledge
* Develop technical reporting and documentation skills
* Understand attacker methodologies and defensive controls

---

## Skills Demonstrated

### Web Security

* Broken Access Control
* SQL Injection (SQLi)
* Command Injection
* HTTP Header Manipulation
* Local File Inclusion (LFI)
* Server-Side Request Forgery (SSRF)
* Authentication Bypass
* Information Disclosure

### Security Testing

* Reconnaissance
* Manual Vulnerability Assessment
* Payload Development
* Request Manipulation
* Exploitation Validation
* Impact Assessment

### Security Analysis

* Root Cause Analysis
* Risk Evaluation
* Attack Surface Analysis
* Security Recommendations

---

## Tools Used

| Tool                   | Purpose                                  |
| ---------------------- | ---------------------------------------- |
| Burp Suite             | Intercepting and modifying HTTP requests |
| Kali Linux             | Security testing environment             |
| Curl                   | API and web request testing              |
| Browser DevTools       | Web application analysis                 |
| Webhook Tester         | Data exfiltration validation             |
| Command Line Utilities | Enumeration and exploitation             |

---

## Challenge Categories

### Web Security

| Challenge     | Vulnerability               |
| ------------- | --------------------------- |
| Broken-eh     | Broken Access Control       |
| Homie         | Header Manipulation         |
| Travelcon     | Command Injection           |
| Ding-Dong     | Command Injection           |
| Library       | SQL Injection               |
| QR Generator  | Remote Command Execution    |
| PDF Generator | Local File Inclusion / SSRF |

### Digital Forensics

* File Analysis
* Data Recovery
* Evidence Investigation
* Artifact Examination

### Cryptography

* Encoding Analysis
* Cipher Identification
* Cryptographic Weakness Analysis

### OSINT

* Open Source Intelligence Investigation
* Information Gathering
* Target Enumeration

---

## Methodology

The following methodology was applied throughout the challenges:

1. Information Gathering
2. Application Enumeration
3. Vulnerability Discovery
4. Exploitation Validation
5. Impact Assessment
6. Security Recommendation
7. Documentation

---

## Key Security Findings

### Broken Access Control

Identified exposed administrative resources and sensitive backup files due to improper access restrictions.

### SQL Injection

Demonstrated how unsanitized user input can lead to unauthorized database access and credential disclosure.

### Command Injection

Identified unsafe command execution mechanisms that could allow arbitrary operating system command execution.

### HTTP Header Trust Issues

Demonstrated bypass techniques through manipulation of trusted HTTP headers.

### Local File Inclusion

Validated the ability to access unintended files from the server filesystem due to insufficient input validation.

---

## Security Impact

The identified vulnerabilities could potentially lead to:

* Unauthorized Access
* Sensitive Information Disclosure
* Account Compromise
* Privilege Escalation
* Remote Code Execution
* Full System Compromise

---

## Key Takeaways

Through these challenges, I gained hands-on experience in:

* Thinking from an attacker's perspective
* Understanding common web vulnerabilities
* Performing vulnerability validation
* Assessing business and technical impact
* Producing structured security reports
* Communicating technical findings effectively

---

## Full Report

📄 Full CTF Writeup Report:

[View PDF Report](https://drive.google.com/file/d/1idkpjALi8a_qTMUIl29eH6oU8L3_DmKQ/view?usp=drive_link)

---

## Disclaimer

This repository is intended solely for educational and portfolio purposes.

All writeups originate from authorized Capture The Flag (CTF) environments. No testing was conducted against unauthorized systems.

---

## Author

**Zaidan Mahfudz Azzam Saidi**

Cybersecurity Student | Security Operations | Vulnerability Assessment | Information Security
