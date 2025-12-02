# Security Scanning

## Overview
This repository uses three types of security scanning:

### SAST (Static Analysis with CodeQL)
- Scans source code for vulnerabilities
- Runs on push to main branch
- Checks for: SQL injection, XSS, command injection, insecure configurations, hardcoded secrets, data flow vulnerabilities
- Artifacts: See GitHub Security tab

### SCA (Dependency Check)
- Scans Python packages for known CVEs
- Runs on push to main branch
- Checks for: Known CVEs in Flask/Werkzeug, outdated packages, transitive dependencies, high-severity vulnerabilities (CVSS ≥ 7.0)
- Artifacts: sca-reports

### DAST (Live Application with ZAP)
- Tests running application for vulnerabilities
- Runs on push to main branch
- Checks for: Missing security headers, server configuration issues, information disclosure, XSS, SQL injection, clickjacking vulnerabilities
- Artifacts: zap-baseline-reports, zap-fullscan-reports

## Reporting Vulnerabilities
Please email security@example.com.
