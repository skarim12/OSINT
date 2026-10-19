<div align="center">

# 🔍 Passive Reconnaissance & OSINT Lab

**Gathering intelligence on a target using only publicly available sources — no direct interaction, no footprint left behind.**

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-OSINT-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Level](https://img.shields.io/badge/Level-Student%20Lab-orange)

</div>

---

## 📖 Overview

**Passive reconnaissance** is the act of gathering information about a target *without* using, notifying, or directly interacting with it. It's typically the first phase of an attack lifecycle — threat actors rely on **Open-Source Intelligence (OSINT)** to build a profile of a target before moving into active reconnaissance, where systems are actually probed and scanned.

This lab walks through the tools and techniques used to build that profile using nothing but public, open sources.

---

## 🛠️ Tools & Techniques

| Tool / Technique | Purpose |
|---|---|
| **Google Dorking** | Advanced search operators (`site`, `inurl`, `link`, `related`, `info`) to uncover subdomains, exposed admin pages, cached content, and third-party connections |
| **WHOIS** | Domain registration lookups for DNS records, IP info, and certificates |
| **nslookup** | CLI queries for MX records and authoritative name servers |
| **theHarvester** | Automated scraping of hosts, IPs, and email addresses from public search engines |
| **Maltego** | Visual link analysis to map domains, employees, and emails via transforms and machines |

---

## 🧭 Walkthrough

1. **Google Dorking** — Used `site:`, `inurl:`, `link:`, `related:`, and `info:` operators to map subdomains and locate an exposed admin page on the target domain
2. **WHOIS & nslookup** — Pulled DNS, MX, and authoritative name server records from the CLI and web lookups
3. **theHarvester** — Collected hosts, IPs, and email addresses across Bing and DuckDuckGo
4. **Maltego** — Ran DNS/email transforms and the *Company Stalker* machine to identify employee emails
5. **Footprinting** — Completed a level-1 footprint: DNS enumeration, DNS resolution, and ASN (Autonomous System Number) resolution

---

## 💡 Key Takeaways

- 🔓 A single exposed admin panel, unsanitized input field, or scraped employee list can hand an attacker everything needed to move into active reconnaissance
- 🔎 Organizations should regularly audit what Google indexes about their own domains
- 🔐 Admin interfaces should be restricted and monitored, not publicly discoverable
- 📧 Scraped employee emails are frequently the foundation of spear-phishing campaigns
- 🛡️ Minimizing public DNS/WHOIS exposure and running security awareness training are critical defensive controls

---

## ⚠️ Disclaimer

> This lab was conducted in a controlled, educational environment against a sample target domain for coursework purposes only. All techniques shown are for **authorized, educational use**. Using these methods against systems without explicit permission is illegal.

---

## 👤 Author

**Saminur Karim**
Cybersecurity Systems @ St. John's University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?logo=linkedin&logoColor=white)](https://linkedin.com/in/saminur-karim-46bb65306)
[![Medium](https://img.shields.io/badge/Medium-black?logo=medium&logoColor=white)](https://medium.com/@karimsaminur123)
[![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white)](https://github.com/karimsaminur123)
