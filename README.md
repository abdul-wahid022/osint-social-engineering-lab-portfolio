<p align="center">
  <img src="images/banner.png" alt="OSINT & Social Engineering Lab Portfolio Banner" width="100%">
</p>

<h1 align="center">OSINT & Social Engineering Lab Portfolio</h1>
<h3 align="center">Reconnaissance, Footprinting & Phishing Simulation Labs — From Passive Recon to Human-Layer Exploitation</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Labs-10-blue?style=flat-square" alt="Labs">
  <img src="https://img.shields.io/badge/OSINT%20Labs-7-informational?style=flat-square" alt="OSINT Labs">
  <img src="https://img.shields.io/badge/Phishing%20Labs-3-red?style=flat-square" alt="Phishing Labs">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
</p>

<p align="center">
  <a href="#overview">Overview</a> ·
  <a href="#osint-and-footprinting">OSINT & Footprinting</a> ·
  <a href="#phishing-and-social-engineering">Phishing & Social Engineering</a> ·
  <a href="#key-results">Key Results</a> ·
  <a href="#tools-used">Tools Used</a> ·
  <a href="#lab-environment">Lab Environment</a> ·
  <a href="#repository-structure">Repository Structure</a> ·
  <a href="#license">License</a> ·
  <a href="#disclaimer">Disclaimer</a> ·
  <a href="#contact">Contact</a>
</p>

---

## Overview

| Item | Detail |
|---|---|
| Focus | Open Source Intelligence (OSINT) gathering, domain/email footprinting, and phishing simulation |
| Total Labs | 10 (7 OSINT · 3 Phishing/Social Engineering) |
| Target | `certifiedhacker.com` (public pentest practice site) and isolated lab/test environments |
| Methodology | Passive recon → active footprinting → automation → social engineering → defensive countermeasure |
| Environment | Kali Linux, Windows 10, isolated virtual lab |

This repository documents hands-on labs covering the reconnaissance and human-layer phases of the penetration testing lifecycle — starting with passive OSINT collection (WHOIS, DNS, Google Dorking, Maltego) and ending with phishing simulation and anti-phishing defense (Gophish, SET, Netcraft).

---

## OSINT and Footprinting

| # | Module | Focus | Report |
|---|---|---|---|
| 01 | [WHOIS & NSLookup](01-OSINT-and-Footprinting/M01-WHOIS-and-NSLookup) | Domain ownership & DNS record footprinting | [Report](01-OSINT-and-Footprinting/M01-WHOIS-and-NSLookup/Lab-Report.pdf) |
| 02 | [Email Header Tracing](01-OSINT-and-Footprinting/M02-Email-Header-Tracing) | Email origin, IP & route tracing (eMailTrackerPro) | [Report](01-OSINT-and-Footprinting/M02-Email-Header-Tracing/Lab-Report.pdf) |
| 03 | [Google Dorking & GHDB](01-OSINT-and-Footprinting/M03-Google-Dorking-and-GHDB) | Search operators & Google Hacking Database recon | [Report](01-OSINT-and-Footprinting/M03-Google-Dorking-and-GHDB/Lab-Report.pdf) |
| 04 | [Pagodo Automation](01-OSINT-and-Footprinting/M04-Pagodo-Automation) | Automated GHDB dork filtering & scanning pipeline | [Report](01-OSINT-and-Footprinting/M04-Pagodo-Automation/Lab-Report.pdf) |
| 05 | [Maltego](01-OSINT-and-Footprinting/M05-Maltego) | Graph-based infrastructure & entity recon | [Report](01-OSINT-and-Footprinting/M05-Maltego/Lab-Report.pdf) |
| 06 | [OSTrICa & OSRFramework](01-OSINT-and-Footprinting/M06-OSTrICa-and-OSRFramework) | Multi-source threat intel aggregation & username recon | [Report](01-OSINT-and-Footprinting/M06-OSTrICa-and-OSRFramework/Lab-Report.pdf) |
| 07 | [Website Mirroring (HTTrack)](01-OSINT-and-Footprinting/M07-Website-Mirroring-HTTrack) | Offline site mirroring & metadata extraction | [Report](01-OSINT-and-Footprinting/M07-Website-Mirroring-HTTrack/Lab-Report.pdf) |

## Phishing and Social Engineering

| # | Module | Focus | Report |
|---|---|---|---|
| 08 | [Gophish Campaign](02-Phishing-and-Social-Engineering/M08-Gophish-Campaign) | End-to-end phishing campaign simulation | [Report](02-Phishing-and-Social-Engineering/M08-Gophish-Campaign/Lab-Report.pdf) |
| 09 | [Social Engineering Toolkit](02-Phishing-and-Social-Engineering/M09-Social-Engineering-Toolkit) | Mass mailer, payload delivery & credential harvesting | [Report](02-Phishing-and-Social-Engineering/M09-Social-Engineering-Toolkit/Lab-Report.pdf) |
| 10 | [Netcraft Anti-Phishing](02-Phishing-and-Social-Engineering/M10-Netcraft-Anti-Phishing) | Defensive countermeasure & phishing detection | [Report](02-Phishing-and-Social-Engineering/M10-Netcraft-Anti-Phishing/Lab-Report.pdf) |

---

## Key Results

| Lab | Result |
|---|---|
| WHOIS & NSLookup | Mapped domain ownership, nameservers & DNS record types |
| Email Header Tracing | Traced sender IP, geolocation & mail routing path from a real header |
| Google Dorking & GHDB | Demonstrated 15+ search operators across 7 GHDB vulnerability categories |
| Pagodo Automation | Reduced 7,944 GHDB dorks to 100 high-priority, target-scoped queries (~98.7% reduction) |
| Maltego | Resolved 7 subdomains, hosting provider, IP geolocation & WHOIS entities in 12 transforms |
| OSTrICa & OSRFramework | Ran multi-plugin domain intel extraction and cross-platform username lookup |
| Website Mirroring | Mirrored full site structure and extracted meta tags, emails & phone numbers |
| Gophish Campaign | Built and launched a full 5-component phishing campaign with tracking |
| SET | Generated a reverse-shell payload, harvested cleartext credentials, and spoofed a trusted link |
| Netcraft | Verified real-time phishing detection, site reputation & IP attribution as a defensive layer |

---

## Tools Used

| Tool | Purpose |
|---|---|
| WHOIS / NSLookup | Domain ownership & DNS record lookup |
| eMailTrackerPro | Email header tracing & IP geolocation |
| Google Search Operators / GHDB | Passive vulnerability discovery |
| Pagodo | Automated GHDB dork scanning |
| Maltego CE | Graph-based OSINT & infrastructure mapping |
| OSTrICa / OSRFramework | Multi-source threat intel & username enumeration |
| HTTrack / Web Data Extractor | Website mirroring & metadata scraping |
| Gophish | Phishing campaign management & tracking |
| Social-Engineer Toolkit (SET) | Payload delivery, mass mailer, credential harvesting |
| Netcraft Extension | Anti-phishing detection & fraud reporting |

---

## Lab Environment

| Component | Detail |
|---|---|
| OS | Kali Linux, Windows 10 |
| Network | Isolated/local lab network (127.0.0.1, local VMs) |
| Target | `certifiedhacker.com` (public pentest practice site) and self-owned test accounts |
| Authorization | All labs performed in a closed, authorized lab environment for educational purposes |

---

## Repository Structure

```
osint-social-engineering-lab-portfolio/
├── README.md
├── LICENSE
├── images/banner.png
├── 01-OSINT-and-Footprinting/
│   ├── README.md
│   ├── images/bannerosint.png
│   ├── M01-WHOIS-and-NSLookup/
│   ├── M02-Email-Header-Tracing/
│   ├── M03-Google-Dorking-and-GHDB/
│   ├── M04-Pagodo-Automation/
│   ├── M05-Maltego/
│   ├── M06-OSTrICa-and-OSRFramework/
│   └── M07-Website-Mirroring-HTTrack/
└── 02-Phishing-and-Social-Engineering/
    ├── README.md
    ├── images/bannersoc.png
    ├── M08-Gophish-Campaign/
    ├── M09-Social-Engineering-Toolkit/
    └── M10-Netcraft-Anti-Phishing/
```

---

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

---

## Disclaimer

All labs in this repository were performed exclusively in a closed, authorized lab environment using the public pentest-practice target `certifiedhacker.com`, self-owned test accounts, and isolated virtual machines. **No real individuals, organizations, or production systems were targeted without consent.** OSINT data (WHOIS/registrant records, email headers) shown in this repository is limited to what is already publicly indexed about the test target; any real third-party personal data, live vulnerable hosts, or exposed credentials surfaced incidentally during labs have been redacted, defanged, or excluded from screenshots and reports. Phishing templates and cloned pages shown here were built and tested only against the author's own accounts/infrastructure and are not intended to impersonate any real brand for malicious use. This repository is for educational and authorized security-training purposes only.

---

## Contact

**Abdul Wahid**
GitHub: [@abdul-wahid022](https://github.com/abdul-wahid022)
