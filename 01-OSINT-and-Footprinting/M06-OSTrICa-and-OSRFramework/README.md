<p align="center">
  <img src="images/cover.png" alt="OSTrICa and OSRFramework Cover" width="100%">
</p>

<h1 align="center">OSINT Collection — OSTrICa & OSRFramework</h1>
<h3 align="center">Multi-Source Threat Intelligence Aggregation & Username Enumeration</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M06-blue?style=flat-square" alt="Module">
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
| Objective | Use OSTrICa to aggregate domain threat intel and OSRFramework to enumerate usernames across platforms |
| Target | `www.certifiedhacker.com` (OSTrICa) and username `analyst` / page `certifiedhacker` (OSRFramework) |
| Platform | Kali Linux, Python 2 (OSTrICa) / Python 3 (OSRFramework) |

## Key Findings

| Tool | Result |
|---|---|
| OSTrICa | Loaded plugins: SafeBrowsing, ThreatCrowd, PyWhois, DomainBigData, BlackLists, ThreatMiner, NortonSafeWeb; some failed (missing deps / SSL error) |
| OSTrICa Graph | Generated an intelligence graph (limited to a single consolidated node due to partial plugin failures) |
| OSRFramework usufy.py | Located username `analyst` on GitHub and Instagram across VK/GitHub/Instagram search |
| OSRFramework searchfy.py | Searched for page `certifiedhacker` across GitHub, Instagram, KeyServerUbuntu — no public subscriber data found |

## Evidence

<p align="center"><img src="images/ostrica-plugin-list-loaded.png" width="80%"></p>
<p align="center"><sub>OSTrICa v0.5 loaded with available plugin list.</sub></p>

<p align="center"><img src="images/ostrica-domain-extraction-run.png" width="80%"></p>
<p align="center"><sub>Intelligence extraction run against www.certifiedhacker.com.</sub></p>

<p align="center"><img src="images/ostrica-generated-graph-browser.png" width="80%"></p>
<p align="center"><sub>Generated intelligence graph opened in browser.</sub></p>

<p align="center"><img src="images/osrframework-usufy-search-result.png" width="80%"></p>
<p align="center"><sub>OSRFramework — usufy.py profile search result across VK, GitHub, Instagram.</sub></p>

## Tools

| Tool | Role |
|---|---|
| OSTrICa | Multi-plugin domain/IP/email/hash threat intelligence collection |
| OSRFramework (usufy.py, searchfy.py) | Username and page-subscriber enumeration across platforms |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to OSINT Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
