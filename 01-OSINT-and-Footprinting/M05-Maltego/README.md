<p align="center">
  <img src="images/cover.png" alt="Maltego CE Cover" width="100%">
</p>

<h1 align="center">OSINT Footprinting — Maltego CE</h1>
<h3 align="center">Graph-Based Infrastructure & Entity Reconnaissance</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M05-blue?style=flat-square" alt="Module">
  <img src="https://img.shields.io/badge/Category-OSINT-informational?style=flat-square" alt="Category">
</p>

<p align="center">
  <a href="#overview">Overview</a> ·
  <a href="#key-findings">Key Findings</a> ·
  <a href="#evidence">Evidence</a> ·
  <a href="#tools">Tools</a> ·
  <a href="Lab-Report.pdf">Full Report</a> ·
  <a href="../README.md">Back</a>
</p>

---

## Overview

| Item | Detail |
|---|---|
| Objective | Run Maltego CE transforms against `www.certifiedhacker.com` to map digital infrastructure |
| Platform | Maltego CE 4.11.2 on Kali Linux |
| Steps Completed | 12 successful transforms (2 CE-version-limited) |

## Key Findings

| Finding | Detail |
|---|---|
| Subdomains | 7 identified (mail, ftp, smtp, pop, imap, webmail, news) |
| Hosting | Bluehost (ns1/ns2.bluehost.com) |
| Server IP | 162.241.216.11 — geolocated to Phoenix, United States |
| Registrar | Network Solutions LLC; registrant shielded via Perfect Privacy LLC |
| Historical data | 25+ Wayback Machine snapshots (2004–2008) |
| CE limitations | Server-Side Technology (BuiltWith) and Open Port transforms unavailable in free edition |

## Evidence

<p align="center"><img src="images/maltego-website-entity-dns-transform.png" width="80%"></p>
<p align="center"><sub>Domain & subdomain identification via DNS transforms.</sub></p>

<p align="center"><img src="images/maltego-ip-geolocation-result.png" width="80%"></p>
<p align="center"><sub>IP address resolution and geolocation to Phoenix, US.</sub></p>

<p align="center"><img src="images/maltego-whois-entities-graph.png" width="80%"></p>
<p align="center"><sub>WHOIS entity graph (registrar, registrant org, address).</sub></p>

<p align="center"><img src="images/maltego-wayback-snapshots-result.png" width="80%"></p>
<p align="center"><sub>Historical Wayback Machine snapshots (2004–2008).</sub></p>

## Tools

| Tool | Role |
|---|---|
| Maltego CE | Entity-relationship OSINT graphing |
| Maltego Transform Hub (Utilities) | DNS, WHOIS, geolocation, Wayback transforms |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to OSINT Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
