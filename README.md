<img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/bf196c22-6d47-4bbc-81b7-465c86511df9" />

# SQL Injection — WHERE Clause Bypass (PortSwigger Lab Write-up)

Vulnerability assessment report documenting a SQL Injection finding in the product category filtering feature of a PortSwigger Web Security Academy lab environment.

## Summary

The application's product category filter passed user input directly into a SQL query without sanitization or parameterization. Submitting `Pets' OR 1=1--` as the category value bypassed the `released = 1` condition, causing the application to return all product records — including unreleased ones that should have been hidden from standard users.

- **Vulnerability class:** SQL Injection (CWE-89)
- **CVSS 3.1 Base Score:** 7.5 (High) — `CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N`
- **Impact:** Unauthorized disclosure of hidden/unreleased data
- **Root cause:** Unparameterized SQL query construction using untrusted input

## Lab Reference

PortSwigger Web Security Academy — *SQL injection vulnerability in WHERE clause allowing retrieval of hidden data*
https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data

## Tools Used

- Burp Suite (Proxy, Repeater)
- Mozilla Firefox

## Contents

| File | Description |
|---|---|
| `Vulnerability_Assessment_Report.pdf` | Full vulnerability assessment report, including PoC screenshots, CVSS scoring, root cause analysis, and remediation recommendations |

## Report Sections

1. Executive Summary
2. Scope & Methodology
3. Vulnerability Analysis (classification, root cause, impact, affected assets, CVSS score)
4. Proof of Concept (testing environment, reproduction steps, expected vs. observed results)
5. Remediation (parameterized queries, defense-in-depth controls, verification steps)

## Disclaimer

This assessment was conducted against an intentionally vulnerable lab environment provided by PortSwigger for authorized security training purposes only. No production systems were tested. This write-up is for educational purposes.

## Author

Taraka Divya Ketha
