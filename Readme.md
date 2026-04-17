# DVWA Vulnerability Assessment & Penetration Testing (VAPT) Report 🛡️

This repository documents a full-scale Vulnerability Assessment and Penetration Testing (VAPT) performed against **Damn Vulnerable Web Application (DVWA)**. The purpose of this assessment is to identify, exploit, and document security vulnerabilities across all DVWA modules and difficulty levels, and provide actionable remediation steps.

---

## 📋 Summary

| Field        | Details                                                      |
|--------------|--------------------------------------------------------------|
| **Target**   | DVWA (Damn Vulnerable Web Application)                       |
| **Scope**    | All vulnerability modules across Low and Medium difficulty   |
| **Tools**    | Burp Suite, OWASP ZAP, Nikto, Hydra, curl, Firefox Dev Tools |
| **Purpose**  | Educational & Ethical Security Research                      |

---

## 🛠️ Vulnerabilities Covered

| #  | Vulnerability               | CWE ID     | CVSS | Risk Level |
|----|-----------------------------|------------|------|------------|
| 1  | Brute-Force Login           | CWE-307    | 8.1  | High       |
| 2  | Command Injection           | CWE-77     | 9.8  | Critical   |
| 3  | Cross-Site Request Forgery  | CWE-352    | 6.5  | Medium     |
| 4  | File Inclusion (LFI)        | CWE-98     | 7.5  | High       |
| 5  | File Upload                 | CWE-434    | 8.8  | High       |
| 6  | Insecure CAPTCHA            | CWE-346    | 5.3  | Medium     |
| 7  | SQL Injection               | CWE-89     | 9.8  | Critical   |
| 8  | Blind SQL Injection         | CWE-89     | 9.0  | Critical   |
| 9  | Weak Session IDs            | CWE-330    | 7.1  | High       |
| 10 | Cross-Site Scripting (XSS)  | CWE-79     | 7.4  | High       |
| 11 | CSP Bypass                  | CWE-693    | 6.1  | Medium     |
| 12 | JavaScript Exploits         | CWE-79/94  | 6.5  | Medium     |
| 13 | Open Redirect               | CWE-601    | 6.1  | Medium     |

---

## 📁 Repository Structure

```
DVWA-VAPT-Report/
├── README.md                             # Project overview and summary
├── Report/
│   ├── DVWA_VAPT_Report.docx             # Full professional report (editable)
│   └── DVWA_VAPT_Report.pdf              # Exported version for sharing
├── Screenshots/                          # Proof-of-concept images per vulnerability
│   ├── BruteForce/
│   ├── CommandInjection/
│   ├── CSRF/
│   ├── FileInclusion/
│   ├── FileUpload/
│   ├── InsecureCAPTCHA/
│   ├── SQLInjection/
│   ├── BlindSQLInjection/
│   ├── WeakSessionIDs/
│   ├── XSS/
│   ├── CSPBypass/
│   ├── JavaScript/
│   └── OpenRedirect/
├── Findings/                             # Individual Markdown report per vulnerability
│   ├── BruteForce.md
│   ├── CommandInjection.md
│   ├── CSRF.md
│   ├── FileInclusion.md
│   ├── FileUpload.md
│   ├── InsecureCAPTCHA.md
│   ├── SQLInjection.md
│   ├── BlindSQLInjection.md
│   ├── WeakSessionIDs.md
│   ├── XSS.md                            # Combined: Reflected, Stored, DOM
│   ├── CSPBypass.md
│   ├── JavaScript.md
│   └── OpenRedirect.md
└── Appendices/
    ├── Tools_Used.md                     # Nmap, Burp Suite, WFuzz, etc.
    ├── Environment_Config.md             # DVWA setup, server stack, OS info
    └── References.md                     # CWE, CVSS, OWASP Top 10 references
```

---

## 🧪 Methodology

1. **Reconnaissance** — Manual exploration of each module across difficulty levels.
2. **Exploitation** — Vulnerabilities exploited using Burp Suite Intruder, curl, and browser-based payloads.
3. **Documentation** — Each finding documented with:
   - CWE ID and CVSS score
   - Detailed proof of concept (PoC)
   - Step-by-step screenshots
   - Actionable remediation recommendations

---

## 🔍 Risk Summary

| Risk Level | Count |
|------------|-------|
| 🔴 Critical | 3    |
| 🟠 High     | 5    |
| 🟡 Medium   | 5    |

---

## 🛡️ Disclaimer

This project is intended **solely for educational and ethical security research purposes**. All testing was performed in a controlled, isolated lab environment against an intentionally vulnerable application.

> ⚠️ Never test real systems or applications without **explicit written permission** from the owner. Unauthorized testing is illegal and unethical.

---

## 📚 References

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CVSS v3.1 Scoring](https://www.first.org/cvss/)
- [CWE List](https://cwe.mitre.org/)
- [DVWA GitHub](https://github.com/digininja/DVWA)

---

