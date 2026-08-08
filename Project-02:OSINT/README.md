# 🔍 OSINT Investigation & Intelligence Gathering

Public data, private conclusions — an Open Source Intelligence investigation of a live website, using only what's already public.


## 🎯 Objective

Investigate a target website using publicly available OSINT resources only — no logins, no scanning, no touching anything not meant to be public — and turn the findings into a professional intelligence report.


## 🧭 What Was Investigated

| Category | What I Looked For |
|----------|-------------------|
| Domain Info | Registrar, registration/expiry dates, domain status |
| WHOIS / RDAP | Ownership records, privacy status, DNSSEC |
| DNS Records | A, AAAA, NS, TXT, SOA, MX |
| Hosting | Provider, ASN, edge/CDN setup |
| SSL/TLS | Issuer, validity, certificate scope, CAA policy |
| Security Headers | CSP, HSTS, X-Frame-Options, and more |
| Tech Stack | Framework, CDN, hosting platform |
| Subdomains | Certificate Transparency, passive DNS, archive search |
| robots.txt / sitemap.xml | Crawl rules, disclosed paths, indexed pages |
| Reputation | Trust score, malware/phishing checks |


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
