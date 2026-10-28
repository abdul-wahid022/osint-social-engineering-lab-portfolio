<p align="center">
  <img src="images/cover.png" alt="WHOIS and NSLookup Cover" width="100%">
</p>

<h1 align="center">Domain Footprinting — WHOIS & NSLookup</h1>
<h3 align="center">Mapping Domain Ownership and DNS Infrastructure</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M01-blue?style=flat-square" alt="Module">
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
| Objective | Perform domain footprinting using WHOIS and nslookup to identify ownership, registration and DNS record data |
| Tools | whois, nslookup (command-line and web-based) |
| Technique | Passive OSINT — no direct interaction with target systems |

## Key Findings

| Finding | Detail |
|---|---|
| WHOIS purpose | Retrieves registrar, registration dates, nameservers and contact details for a domain |
| WHOIS flags covered | `-h` (host), `-p` (port), `-H` (hide disclaimer), `-i` (inverse lookup), `-T` (type), `-K` (connected), `-B` (bulk), `-r` (raw), `-v` (verbose), `-V` (version) |
| nslookup purpose | Queries DNS servers for A, AAAA, MX, NS and other record types |
| nslookup modes | Non-interactive (single query) and interactive (multi-query shell) |
| Use cases | Security analysis, DNS troubleshooting, domain verification, network diagnostics |

## Evidence

<p align="center"><img src="images/whois-command-syntax-example.png" width="80%"></p>
<p align="center"><sub>Example WHOIS command-line query and flag usage.</sub></p>

<p align="center"><img src="images/whois-web-based-lookup-tool.png" width="80%"></p>
<p align="center"><sub>Web-based WHOIS lookup tool interface.</sub></p>

<p align="center"><img src="images/nslookup-basic-query-output.png" width="80%"></p>
<p align="center"><sub>Basic nslookup query output showing resolved DNS records.</sub></p>

## Tools

| Tool | Role |
|---|---|
| whois | Domain registration & ownership lookup |
| nslookup | DNS record querying and troubleshooting |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to OSINT Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
