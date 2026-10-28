<p align="center">
  <img src="images/cover.png" alt="Website Mirroring and Metadata Extraction Cover" width="100%">
</p>

<h1 align="center">Website Footprinting & Metadata Extraction</h1>
<h3 align="center">Offline Site Mirroring (HTTrack) and Metadata Scraping (Web Data Extractor)</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M07-blue?style=flat-square" alt="Module">
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
| Objective | Mirror `certifiedhacker.com` offline with HTTrack and extract metadata/contacts with Web Data Extractor |
| Tools | HTTrack (WinHTTrack 3.49-2), Web Data Extractor 8.3 |
| Platform | Windows |

## Key Findings

| Finding | Detail |
|---|---|
| HTTrack mirror | Full site structure, HTML/CSS/JS and images copied locally; login form, image paths and internal links exposed |
| Directory analysis | Confirmed plain HTML/CSS/JS stack with no visible server-side framework |
| Web Data Extractor | Crawled site in a single session: 47 meta tags, 6 emails, 23 phone numbers, 21 fax numbers, 481 URLs |
| Use case | Contact/metadata extraction flagged as valuable for social engineering / spear-phishing / vishing profiling |

## Evidence

<p align="center"><img src="images/httrack-mirrored-site-browser-view.png" width="80%"></p>
<p align="center"><sub>Mirrored certifiedhacker.com opened locally — functions identically to the live site.</sub></p>

<p align="center"><img src="images/httrack-directory-structure-tree.png" width="80%"></p>
<p align="center"><sub>Internal directory structure revealed after mirroring.</sub></p>

<p align="center"><img src="images/web-data-extractor-session-settings.png" width="80%"></p>
<p align="center"><sub>Web Data Extractor session configuration for certifiedhacker.com crawl.</sub></p>

<p align="center"><img src="images/web-data-extractor-results-summary-tabs.png" width="80%"></p>
<p align="center"><sub>Extraction results summary — meta tags, emails, phones, URLs tab counts.</sub></p>

## Tools

| Tool | Role |
|---|---|
| HTTrack (WinHTTrack) | Full offline website mirroring |
| Web Data Extractor 8.3 | Meta tag, email, phone, fax and URL scraping |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to OSINT Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
