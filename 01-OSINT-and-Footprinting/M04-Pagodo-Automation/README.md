<p align="center">
  <img src="images/cover.png" alt="Pagodo Automation Cover" width="100%">
</p>

<h1 align="center">Automated Passive Recon — Pagodo & GHDB Dork Automation</h1>
<h3 align="center">Scaling Google Dorking with Priority-Based Python Automation</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M04-blue?style=flat-square" alt="Module">
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
| Objective | Automate GHDB dork scraping, filtering and prioritized scanning using Pagodo and custom Python scripts |
| Target | Test-lab-scoped target domain (used as a filtering/automation demo, test environment) |
| Pipeline | GHDB scrape → filter → priority-rank → auto-scope → scan |

## Key Findings

| Step | Result |
|---|---|
| GHDB Dorks Scraped | 7,944 total |
| Custom Filter Script | Reduced to 4,181 relevant dorks (52.6% reduction) |
| Smart Priority Script | Ranked into High/Medium/Low tiers; top 100 auto-selected and auto-scoped with `site:` |
| Rate-Limit Handling | Pagodo correctly detected Google IP block and auto-slept 60 minutes before resuming |
| Output | JSON + TXT result files and full scan log generated |

## Evidence

<p align="center"><img src="images/pagodo-ghdb-scraper-execution.png" width="80%"></p>
<p align="center"><sub>ghdb_scraper.py pulling the full GHDB dork library.</sub></p>

<p align="center"><img src="images/filter-dorks-script-output.png" width="80%"></p>
<p align="center"><sub>filter_dorks.py output: 7,944 → 4,181 relevant dorks.</sub></p>

<p align="center"><img src="images/smart-dork-priority-tiers.png" width="80%"></p>
<p align="center"><sub>smart_dork.py priority-tier ranking and top-100 selection.</sub></p>

<p align="center"><img src="images/pagodo-rate-limit-handling-log.png" width="80%"></p>
<p align="center"><sub>Pagodo log showing Google IP-block detection and automatic 60-minute sleep/resume.</sub></p>

## Tools

| Tool | Role |
|---|---|
| Pagodo | Automated GHDB dork scanning against a target |
| Python (custom scripts) | Dork filtering and priority-based ranking |
| Git | Cloning Pagodo from GitHub |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to OSINT Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
