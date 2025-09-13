# OWASP Juice Shop — Findings Summary

**Project:** OWASP Juice Shop — Penetration Test  

**Author:** Silent_Root , Naggar

**Contents:** brief, non-exploitable summaries of validated findings. The full technical **REPORT** (`Owasp juice - Web pentest report v2.0.docx`) is included in this repository and contains scope, redacted reproduction steps, severity (CVSS where applicable), and remediation guidance for authorized reviewers.

---

## Validated Findings (summary)

- **Abusing functionality of AI Chatbot**  
  Identified misuse cases where the chatbot functionality can be manipulated to return sensitive or unintended information. Investigation focused on input handling and response generation behavior.

- **Admin Registration Bypass**  
  Found a weakness in the registration/authorization flow that allowed escalation of privileges under lab conditions (bypassing intended admin-registration controls). Details and remediation are in the report.

- **Broken Access Control on Cart**  
  Observed access control weaknesses allowing unauthorized access or modification of cart data between users (improper enforcement of authorization checks).

- **Brute Force on Admin Password**  
  Demonstrated that the admin login was susceptible to automated password-guessing under lab settings due to missing/insufficient brute-force protections (rate limiting, account lockout, CAPTCHAs).

- **Enumeration to Find Admin Path**  
  Used safe enumeration techniques to discover hidden/admin interface endpoints. Enumeration findings were used to define scope for follow-up tests.

- **Improper Input Validation in Registration Page**  
  Registration inputs were insufficiently validated/sanitized, enabling injection-style payloads or unexpected application behavior in the lab environment.

- **SQL Injection in Login**  
  A login-related input was validated as vulnerable to SQL injection in the test instance. The issue was validated and documented in the report with redacted PoC details.

- **XSS on Search**  
  Cross-site scripting was identified in the search functionality (reflected/stored behavior depending on the vector). Public PoCs are redacted; see report for controlled reproduction steps.

---

## What's included in this repo
- `Owasp juice - Web pentest report v2.0.docx` — Full technical report (redacted/non-exploitable PoCs, severity, remediation).
- Individual markdown writeups for each finding (e.g., `SQLI in login.md`, `XSS on Search.md`, etc.).

---
