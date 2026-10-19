Passive Reconnaissance & OSINT Lab
A hands-on cybersecurity lab demonstrating passive reconnaissance techniques used to gather information about a target without direct interaction with its systems.
Overview
Passive reconnaissance is the first phase in a typical attack lifecycle, gathering publicly available information (OSINT) about a target before any active scanning or exploitation begins. This lab walks through the tools and techniques a threat actor — or a penetration tester — uses to build a profile of a target domain using only open, public sources.
Tools & Techniques
Google Dorking — Advanced search operators (site, inurl, link, related, info) to find subdomains, exposed admin pages, cached content, and third-party connections
WHOIS — Domain registration lookups for DNS records, IP information, and certificates
nslookup — CLI queries for MX records and authoritative name servers
theHarvester — Automated scraping of hosts, IPs, and email addresses from public search engines (Bing, DuckDuckGo)
Maltego — Visual link analysis to map domains, employees, and email addresses using transforms and machines (e.g., Company Stalker)
What I Did
Used Google Dork operators to map subdomains and locate an exposed admin page on the target domain
Ran WHOIS and nslookup to pull DNS, MX, and name server records
Used theHarvester to collect hosts, IPs, and email addresses across multiple search engines
Used Maltego to run DNS/email transforms and a Company Stalker machine to identify employee emails
Completed a level-1 footprint including DNS enumeration, DNS resolution, and ASN resolution
Key Takeaways
A single exposed admin panel, unsanitized input field, or scraped employee list can give an attacker everything needed to move into active reconnaissance
Organizations should audit what Google indexes about their own domains and restrict public access to admin interfaces
Employee emails and contact info gathered via OSINT are frequently the foundation of spear-phishing campaigns
Minimizing public DNS/WHOIS exposure and running regular security awareness training are key defensive controls
Author
Saminur Karim
Cybersecurity Systems, St. John’s University
