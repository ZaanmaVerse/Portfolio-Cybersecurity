# 🛡️ Third-Party Security Risk Assessment: SOC Procurement (Wazuh SIEM)

## 📌 Project Overview
This project is an **Independent Case Study** leveraging my experience as a Cybersecurity Team Intern at **PTPN**. It simulates a **Third-Party Risk Management (TPRM)** security assessment conducted on **PT PGAS**, a prospective vendor providing *Managed Security Operations Center (SOC)* services powered by the **Wazuh Enterprise SIEM** platform.

The primary objective of this assessment is to evaluate the vendor's technical architecture, log data governance, regulatory compliance (**ISO 27001** & **UU PDP/Indonesian Privacy Law**), and operational resilience prior to integrating their services into PT PTPN's critical infrastructure.

---

## 📊 Assessment Summary & Methodology
The evaluation assessed **10 Core Security Controls** utilizing a semi-quantitative approach (*Likelihood vs Impact*) to determine the overall risk posture.

*   **Overall Risk Score:** 🟡 **MEDIUM RISK (2.8 / 5.0)**
*   **Key Findings:** 1 High-Risk vulnerability, 3 Medium-Risk vulnerabilities, and 6 Low-Risk compliant controls.
*   **Final Decision:** **Conditional Approval** (Approved subject to the fulfillment of the remediation action plan).

---

## 🔗 Live Artifacts & Deliverables
The complete comprehensive risk register, executive summary, and remediation timeline can be accessed directly via the link below:

👉 **[Live Project Spreadsheet (Google Sheets)](https://docs.google.com/spreadsheets/d/1DAQqPs0kX02aA00nmBm107aQDxgYr4jUiqGp3AZ_MRI/edit?usp=sharing)**

*The spreadsheet is fully structured with three core tabs: Executive Summary, Vendor Risk Questionnaire (10 Audited Controls), and the Action Remediation Plan.*

---

## 🔍 Key Risk Findings & Solutions

### 1. Critical: 90-Day Log Retention Limitation (High Risk)
*   **Impact:** PT PTPN risks losing crucial digital forensic evidence during long-term cyber attacks, such as *Advanced Persistent Threats (APTs)*, which often go undetected for months.
*   **GRC Solution:** Mandated PT PGAS to upscale the cold storage log retention capacity specifically for PT PTPN to **minimum 365 days (1 year)** prior to signing the contract.

### 2. High: 60-Minute Incident Response SLA (Medium Risk)
*   **Impact:** A 1-hour window for critical alerts (e.g., *Ransomware* outbreaks) is too broad and could lead to widespread lateral movement across PTPN's factory operational network.
*   **GRC Solution:** Renegotiated the SLA clause in the service agreement to reduce the critical incident escalation time to a **maximum of 15-30 minutes**.

### 3. High: Lack of Enforced Multi-Factor Authentication (Medium Risk)
*   **Impact:** Compromised credentials of a remote-working PGAS SOC analyst could grant threat actors unauthorized access to PTPN's vulnerability metrics and network maps via the Wazuh dashboard.
*   **GRC Solution:** Enforced a mandatory IAM policy requiring MFA for all vendor SOC personnel before system integration.

---

## 🛠️ Skills & Standards Demonstrated
*   **Frameworks & Regulations:** ISO/IEC 27001 (ISMS Standards), Law No. 27/2022 on Personal Data Protection (UU PDP).
*   **Technical Knowledge:** Security Operations Center (SOC) Architecture, Wazuh SIEM Architecture, Log Governance, Identity & Access Management (MFA/RBAC).
*   **Analytical Skills:** Risk Assessment, Third-Party Risk Management (TPRM), Audit Methodology, Vendor Evaluation, Strategic Remediation Planning.

---
💡 *Note: This document is crafted solely for professional portfolio purposes using simulated scenario metrics to maintain institutional confidentiality.*
