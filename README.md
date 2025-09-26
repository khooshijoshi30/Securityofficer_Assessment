# Securityofficer_Assessment
# Security Assessment – http://www.itsecgames.com/

This repository contains the assessment work for the Security Officer Trainee problem statement.

---

## 📜 Problem Statement
Evaluate the security posture of `http://www.itsecgames.com`:
- Identify vulnerabilities and misconfigurations.
- Assess SSL/TLS configuration.
- Highlight exposed information from headers, banners, and error messages.
- Provide prioritized mitigation recommendations.

---

## 🛠 Tools Used
| Tool | Purpose |
|-------|---------|
| Nmap | Network and service scanning, version detection |
| OWASP ZAP | Passive scanning of web application and security headers |
| SSL Labs Test | External TLS/SSL configuration assessment |
| PowerShell Headers | Retrieve HTTP headers and server banners |

---

## 📂 Repository Structure
Security_Assessment_Itsecgames/
├── README.md
├── Security_Assessment_Report_Clean.docx
├── Reports/
│ ├── nmapscan.pdf
│ ├── SSL_Server_Test.pdf
│ ├── ZAP_Scanning_Report.pdf
└── Screenshots/
├── headers_screenshot.png

---

## 🔍 Summary of Key Findings

| Finding | Evidence | Risk | Recommendation |
|---------|----------|------|----------------|
| Server type disclosed (Apache) | Server header from PowerShell | Medium | Hide server version/banner in Apache config |
| Missing HSTS and CSP headers | OWASP ZAP report | High | Add modern security headers (HSTS, CSP, X-Frame-Options, X-Content-Type-Options) |
| ETag and Last-Modified headers exposed | PowerShell headers | Low | Remove/rotate ETags, update application regularly |
| Outdated TLS versions (if any) | SSL Labs report | High | Disable TLS 1.0/1.1, enable only TLS 1.2+ |

---

## 📑 Reports Included

- **Security_Assessment_Report_Clean.docx** – Main documented report (problem statement, methodology, findings, recommendations).
- **Reports/nmapscan.pdf** – Nmap Scan Report.
- **Reports/ZAP_Scanning_Report.pdf** – OWASP ZAP Scanning Report.
- **Reports/SSL_Server_Test.pdf** – SSL Labs Test Report.
- **Screenshots/headers_screenshot.png** – Evidence of HTTP headers.

---

## 📝 How to View
- Open the `Security_Assessment_Report_Clean.docx` for the documented findings.
- Navigate to the `Reports/` folder for the full scan reports.
- View `Screenshots/` for evidence screenshots.

---

## 🖥 Video Demonstration


---

## 👤 Author
- Khooshi Joshi  
- Security Officer Trainee Assignment

