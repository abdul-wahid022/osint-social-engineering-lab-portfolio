<p align="center">
  <img src="images/bannerosint.png" alt="OSINT and Footprinting Banner" width="100%">
</p>

<h1 align="center">OSINT and Footprinting</h1>
<h3 align="center">Passive & Active Reconnaissance — Domain, Email, Search Engine and Infrastructure Footprinting</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Labs-7-blue?style=flat-square" alt="Labs">
  <img src="https://img.shields.io/badge/Category-OSINT-informational?style=flat-square" alt="Category">
</p>

<p align="center">
  <a href="#overview">Overview</a> ·
  <a href="#labs">Labs</a> ·
  <a href="#recon-workflow">Recon Workflow</a> ·
  <a href="../README.md">Back to Main Repo</a>
</p>

---

## Overview

This section covers the passive and active reconnaissance phase of OSINT: identifying domain ownership, DNS infrastructure, email origin, exposed files/directories via search engines, graph-based entity mapping, and full offline website mirroring — all performed against the public pentest-practice target `certifiedhacker.com`.

## Labs

| # | Module | Tool(s) | Key Output |
|---|---|---|---|
| 01 | [WHOIS & NSLookup](M01-WHOIS-and-NSLookup) | whois, nslookup | Domain registrar, nameservers, DNS record types |
| 02 | [Email Header Tracing](M02-Email-Header-Tracing) | eMailTrackerPro | Sender IP, geolocation, mail route |
| 03 | [Google Dorking & GHDB](M03-Google-Dorking-and-GHDB) | Google Search Operators, Exploit-DB GHDB | Exposed files/panels via dorks |
| 04 | [Pagodo Automation](M04-Pagodo-Automation) | Pagodo, Python | Automated, priority-ranked dork scanning |
| 05 | [Maltego](M05-Maltego) | Maltego CE | Subdomains, IP, hosting, WHOIS graph |
| 06 | [OSTrICa & OSRFramework](M06-OSTrICa-and-OSRFramework) | OSTrICa, OSRFramework | Multi-source domain intel, username lookup |
| 07 | [Website Mirroring](M07-Website-Mirroring-HTTrack) | HTTrack, Web Data Extractor | Full site mirror, meta tags/emails/phones |

## Recon Workflow

Each tool in this section feeds the next, building a progressively fuller picture of the target:

| Stage | Tool | Feeds Into |
|---|---|---|
| 1. Ownership | WHOIS & NSLookup | Admin emails/phones → Email Header Tracing; nameservers/IP → Maltego |
| 2. Email Trail | Email Header Tracing | Confirms mail infrastructure found via WHOIS/Maltego MX records |
| 3. Exposure Discovery | Google Dorking & GHDB | Manual dork patterns reused and scaled in Pagodo Automation |
| 4. Automation | Pagodo | Scales Stage 3 across thousands of dorks with priority ranking |
| 5. Infrastructure Graph | Maltego | Consolidates DNS, IP, geolocation, WHOIS into one entity graph |
| 6. Cross-Source Intel | OSTrICa & OSRFramework | Aggregates threat-intel feeds and social/username footprints |
| 7. Offline Analysis | Website Mirroring (HTTrack) | Captures full site structure, source code & contact data for static review |

---

<p align="center"><a href="../README.md">⬅ Back to Main Repository</a></p>
