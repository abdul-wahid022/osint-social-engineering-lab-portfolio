<p align="center">
  <img src="images/cover.png" alt="Google Dorking and GHDB Cover" width="100%">
</p>

<h1 align="center">Passive OSINT — Google Dorking & GHDB</h1>
<h3 align="center">Search Operators and the Google Hacking Database for Exposure Discovery</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M03-blue?style=flat-square" alt="Module">
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
| Objective | Demonstrate Google search operators and navigate GHDB categories to identify publicly exposed vulnerabilities |
| Platform | Exploit-DB Google Hacking Database (7,944+ dorks, as of 2026) |
| Scope | Basic & intermediate operators, plus live GHDB category walkthroughs |

## Key Findings

| Operator / Category | Purpose |
|---|---|
| `site:`, `inurl:`, `intitle:`, `intext:` | Domain, URL, title and body-content scoping |
| `filetype:` / `ext:` | Locating exposed file types (pdf, sql, env, log, bak) |
| `cache:`, `-`, `" "`, `*`, `OR` | Cached views, exclusion, exact phrase, wildcard, boolean OR |
| `allinurl:`, `allintitle:`, `allintext:`, `related:`, `info:`, `define:`, `numrange:` | Intermediate precision operators |
| GHDB categories covered | Footholds, Files Containing Usernames, Sensitive Directories, Web Server Detection, Vulnerable Files, Vulnerable Servers, Error Messages |

## Evidence

<p align="center"><img src="images/ghdb-category-footholds-result.png" width="80%"></p>
<p align="center"><sub>GHDB "Footholds" category — example dork and result structure.</sub></p>

<p align="center"><img src="images/intitle-index-of-directory-listing.png" width="80%"></p>
<p align="center"><sub>`intitle:"index of"` dork demonstrating open directory listing discovery.</sub></p>

<p align="center"><img src="images/ghdb-web-server-detection-category.png" width="80%"></p>
<p align="center"><sub>GHDB "Web Server Detection" category — default server page exposure.</sub></p>

<p align="center"><img src="images/ghdb-error-messages-category.png" width="80%"></p>
<p align="center"><sub>GHDB "Error Messages" category — information leakage via application errors.</sub></p>

> 🔒 Hostnames referenced in the full report should be defanged (e.g. `example[.]com`) rather than left as clickable links.

## Tools

| Tool | Role |
|---|---|
| Google Search Operators | Manual precision search queries |
| Exploit-DB GHDB | Categorized community dork repository |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to OSINT Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
