# Authentication Failure Assessment – Account Confusion via Username Normalization

## Overview

This project documents a hands-on security assessment conducted as part of the TryHackMe OWASP Top 10 (2025) learning path, specifically within **A07: Authentication Failures (IAAA Failures)**.

The objective of this exercise was to identify weaknesses in the application's authentication and account management process that could allow unauthorized access to privileged accounts through inconsistent username handling and normalization.

---

## Learning Objectives

* Understand common authentication-related vulnerabilities.
* Identify weaknesses in username validation and account registration processes.
* Assess the impact of improper identity handling during authentication.
* Learn how inconsistent username normalization can lead to privilege escalation.
* Practice documenting authentication security findings in a professional format.

---

## Scenario

A simulated online banking application provides user registration and login functionality.

During testing, it was observed that the application allowed registration using a username visually similar to an existing privileged account by altering character casing.

Example:

```text id="p7d4e8"
Original Account : admin
Registered Account : aDmiN
```

After registration and authentication, the application treated the newly created account as the privileged account, resulting in unauthorized access to administrative resources.

This behavior indicates a flaw in how the application handles username uniqueness and authentication identity validation.

---

## Methodology

### 1. Reconnaissance

* Reviewed the application's registration and login functionality.
* Identified the existence of a privileged account named `admin`.
* Observed how usernames were processed during registration.

### 2. Analysis

* Tested account registration using variations of the existing privileged username.
* Evaluated whether the application enforced case-sensitive uniqueness checks.
* Investigated how usernames were normalized during authentication.

### 3. Validation

* Successfully registered an account using a case-modified version of an existing privileged username.
* Authenticated using the newly created account.
* Confirmed that access was granted to resources associated with the privileged account.

### 4. Documentation

* Recorded observations and screenshots.
* Assessed potential business impact.
* Documented remediation recommendations.

---

## Findings

### Finding 1: Authentication Confusion Through Improper Username Normalization

**Category:** OWASP Top 10 (2025) – A07: Authentication Failures

The application failed to properly enforce unique identity validation during user registration.

A user was able to register an account using a variation of an existing privileged username by changing letter casing.

Example:

```text id="3n4z7x"
admin
aDmiN
AdMiN
ADMIN
```

Although these usernames appear different from a technical perspective, the authentication system later normalized or interpreted them as the same identity.

As a result, the attacker gained access to resources associated with the privileged account.

---

## Impact

If exploited in a real-world environment, this vulnerability could lead to:

* Unauthorized access to privileged accounts.
* Account takeover scenarios.
* Privilege escalation.
* Exposure of sensitive information.
* Financial fraud and unauthorized transactions.
* Regulatory and compliance violations.
* Reputational damage.

**Risk Severity:** High

---

## Evidence

### Observation 1 – Account Registration

A new account was successfully registered using a username visually similar to an existing privileged account.

Example:

```text id="g8v6s2"
Username: aDmiN
Password: ********
```

### Observation 2 – Authentication

The newly created account successfully authenticated into the application.

### Observation 3 – Unauthorized Privileged Access

After authentication, the application displayed resources associated with the privileged account.

Observed indicators included:

* Administrative account information.
* Elevated account privileges.
* Sensitive account data exposure.

### Screenshot Evidence

#### Registration Process

```text id="5m7f8x"
screenshots/registration.png
```

#### Authentication Process

```text id="8j2k4n"
screenshots/login.png
```

#### Unauthorized Account Access

```text id="9v4e2w"
screenshots/account-dashboard.png
```

### Security Observation

The application failed to maintain a consistent identity management process between registration and authentication components.

Usernames were handled differently across the application lifecycle, resulting in identity confusion and unauthorized account access.

---

## Remediation

### 1. Enforce Case-Insensitive Username Uniqueness

Usernames should be normalized before storage and uniqueness validation.

Example:

```text id="w3r5y7"
admin
ADMIN
AdMiN
aDmiN
```

All should be treated as the same identifier.

---

### 2. Normalize Usernames During Registration

Convert usernames into a standardized format before saving them.

Example:

```text id="t6u8i0"
Input  : aDmiN
Stored : admin
```

---

### 3. Implement Strong Identity Validation

Ensure that authentication processes reference a unique internal identifier rather than relying solely on username matching.

---

### 4. Perform Secure Account Enumeration Controls

Prevent attackers from identifying existing privileged usernames through registration behavior.

---

### 5. Conduct Authentication Security Testing

Regularly assess authentication workflows to identify:

* Account confusion vulnerabilities.
* Authentication bypass scenarios.
* Privilege escalation paths.

---

## Skills Demonstrated

* Authentication Security Assessment
* Identity Management Analysis
* Access Control Validation
* Vulnerability Analysis
* Risk Assessment
* Security Documentation
* Security Reporting
* OWASP Top 10 Mapping

---

## Tools Used

* Web Browser
* Browser Developer Tools
* Manual Authentication Testing
* TryHackMe Lab Environment

---

## Key Takeaways

* Authentication systems must handle usernames consistently throughout registration and login workflows.
* Identity normalization errors can lead to severe authentication bypass vulnerabilities.
* Privileged accounts require additional protection mechanisms beyond simple username validation.
* Small implementation flaws in authentication logic can result in full account compromise.
* Authentication Failures remain a critical category within OWASP Top 10 due to their potential impact on confidentiality, integrity, and access control.

---

## OWASP Mapping

| Category                | Classification                                         |
| ----------------------- | ------------------------------------------------------ |
| OWASP Top 10 (2025)     | A07: Authentication Failures                           |
| Vulnerability Type      | Authentication Confusion / Username Normalization Flaw |
| Risk Level              | High                                                   |
| Impact                  | Unauthorized Account Access                            |
| Attack Complexity       | Low                                                    |
| Authentication Required | No (Registration Only)                                 |

---

## Disclaimer

This project was completed in a controlled educational environment provided by TryHackMe for cybersecurity learning purposes. No real systems or sensitive data were accessed during this exercise.
