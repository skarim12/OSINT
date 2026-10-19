🔍 Passive Reconnaissance & OSINT Lab
Gathering intelligence on a target using only publicly available sources — no direct interaction, no footprint left behind.
Show Image Show Image Show Image
</div>
📖 Overview
Passive reconnaissance is the act of gathering information about a target without using, notifying, or directly interacting with it. It's typically the first phase of an attack lifecycle — threat actors rely on Open-Source Intelligence (OSINT) to build a profile of a target before moving into active reconnaissance, where systems are actually probed and scanned.
This lab walks through the tools and techniques used to build that profile using nothing but public, open sources.
🛠️ Tools & Techniques
Tool / Technique	Purpose
Google Dorking	Advanced search operators (site, inurl, link, related, info) to uncover subdomains, exposed admin pages, cached content, and third-party connections
WHOIS	Domain registration lookups for DNS records, IP info, and certificates
nslookup	CLI queries for MX records and authoritative name servers
theHarvester	Automated scraping of hosts, IPs, and email addresses from public search engines
Maltego	Visual link analysis to map domains, employees, and emails via transforms and machines
🧭 Walkthrough
Google Dorking — Used site:, inurl:, link:, related:, and info: operators to map subdomains and locate an exposed admin page on the target domain
WHOIS & nslookup — Pulled DNS, MX, and authoritative name server records from the CLI and web lookups
theHarvester — Collected hosts, IPs, and email addresses across Bing and DuckDuckGo
Maltego — Ran DNS/email transforms and the Company Stalker machine to identify employee emails
Footprinting — Completed a level-1 footprint: DNS enumeration, DNS resolution, and ASN (Autonomous System Number) resolution
💡 Key Takeaways
🔓 A single exposed admin panel, unsanitized input field, or scraped employee list can hand an attacker everything needed to move into active reconnaissance
🔎 Organizations should regularly audit what Google indexes about their own domains
🔐 Admin interfaces should be restricted and monitored, not publicly discoverable
📧 Scraped employee emails are frequently the foundation of spear-phishing campaigns
🛡️ Minimizing public DNS/WHOIS exposure and running security awareness training are critical defensive controls
⚠️ Disclaimer
This lab was conducted in a controlled, educational environment against a sample target domain for coursework purposes only. All techniques shown are for authorized, educational use. Using these methods against systems without explicit permission is illegal.
👤 Author
Saminur Karim Cybersecurity Systems @ St. John's University
LinkedIn Medium GitHub
