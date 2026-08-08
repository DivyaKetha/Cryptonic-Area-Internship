# 🔍 OSINT Investigation & Intelligence Gathering

Public data, private conclusions — an Open Source Intelligence investigation of a live website, using only what's already public.


## 🎯 Objective

Investigate a target website using publicly available OSINT resources only — no logins, no scanning, no touching anything not meant to be public — and turn the findings into a professional intelligence report.

## | Category | Findings |
|----------|----------|
| **Domain Info** | • Registrar: [Insert]<br>• Registration Date: [Insert]<br>• Expiry Date: [Insert]<br>• Domain Status: [Insert] |
| **WHOIS / RDAP** | • Ownership: [Public/Privacy Protected]<br>• Registrant: [Insert]<br>• DNSSEC: [Signed/Unsigned]<br>• Privacy Service: [Yes/No] |
| **DNS Records** | • A/AAAA: [Insert IPs]<br>• NS: [Insert]<br>• TXT: [Insert SPF/DKIM/DMARC]<br>• SOA: [Insert]<br>• MX: [Insert] |
| **Hosting** | • Provider: [Insert]<br>• ASN: [Insert]<br>• CDN: [Insert]<br>• Edge Network: [Yes/No] |
| **SSL/TLS** | • Issuer: [Insert]<br>• Validity: [Insert Dates]<br>• Certificate Type: [DV/OV/EV]<br>• CAA Policy: [Configured/Missing]<br>• Wildcard: [Yes/No] |
| **Security Headers** | • CSP: [Configured/Missing]<br>• HSTS: [Enabled/Disabled]<br>• X-Frame-Options: [DENY/SAMEORIGIN/ALLOW]<br>• X-Content-Type-Options: [nosniff/Missing]<br>• Referrer-Policy: [Configured/Missing] |
| **Tech Stack** | • Framework: [Insert]<br>• Web Server: [Insert]<br>• CMS: [Insert]<br>• Analytics: [Insert] |
| **Subdomains** | • Discovered: [Count]<br>• Notable: [List]<br>• Source: [CT logs/Passive DNS/Archive]<br>• Active: [List] |
| **robots.txt / sitemap** | • robots.txt: [Present/Missing]<br>• Disallowed: [List paths]<br>• Sitemap: [Present/Missing]<br>• Exposed Paths: [List if found] |
| **Reputation** | • Trust Score: [High/Medium/Low]<br>• Malware: [Clean/Flagged]<br>• Phishing: [Clean/Reported]<br>• Blacklists: [Not listed/Listed] |


## 🛠️ Toolkit

```DomainTools 
ICANN Lookup
(RDAP) who.is
Wappalyzer
securityheaders.com
VirusTotal
crt.sh
Wayback Machine
ScamAdviser
```

Every tool used, and exactly what it was used for, is documented in the report's Source Documentation section — each finding is traceable back to where it came from.

## 🔐 A Note on Privacy

This repo doesn't include raw screenshots or the target's actual data. Treating what you find during OSINT with the same care you'd want your own data treated is part of doing this properly, not an afterthought. The full report (shared separately / with instructor) contains the complete evidence trail.

## 📄 Deliverable

A structured intelligence report covering:

Executive Summary
Target Overview & Methodology
Information Gathered (10+ categories)
Source Documentation (tool + URL per finding)
Security Observations & why each one matters
Recommendations

## 🧠 What I Learned

OSINT depends on cross-checking multiple free tools — no single source gives the full picture. A wildcard SSL certificate can hide subdomains from tools like crt.sh, and testing the wrong URL (a redirect instead of the live page) can quietly produce misleading results. Most of all: a surprising amount of security-relevant information is public — the skill is knowing where to look, and knowing what not to publish.
