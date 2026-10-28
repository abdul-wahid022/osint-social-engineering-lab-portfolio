<p align="center">
  <img src="images/cover.png" alt="Netcraft Anti-Phishing Cover" width="100%">
</p>

<h1 align="center">Anti-Phishing Defense — Netcraft Browser Extension</h1>
<h3 align="center">Real-Time Phishing Detection, Site Intelligence & Fraud Reporting</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M10-red?style=flat-square" alt="Module">
  <img src="https://img.shields.io/badge/Category-Phishing%20Defense-success?style=flat-square" alt="Category">
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
| Objective | Install and use the Netcraft browser extension as a defensive countermeasure against the Gophish/SET techniques |
| Platform | Firefox Add-Ons Store |
| Target tested | certifiedhacker.com (inline panel), netcraft.com (full site report reference) |

## Key Findings

| Finding | Detail |
|---|---|
| Site Report Panel | Shows country, site rank, first-seen date and host at a glance |
| Full Site Report | Background, network, IP delegation and geolocation data |
| IP Delegation | Traced IANA → regional registry → final network block owner |
| Geolocation | Multilateration-based server location, more reliable than simple IP lookup |
| Fraud Reporting | Built-in one-click submission of suspicious URLs to Netcraft's takedown team |
| Defensive mapping | Directly counters Gophish/SET techniques via First-Seen date and IP attribution |

## Evidence

<p align="center"><img src="images/netcraft-extension-installed-firefox.png" width="80%"></p>
<p align="center"><sub>Netcraft Extension installed and active in Firefox.</sub></p>

<p align="center"><img src="images/netcraft-inline-site-report-panel.png" width="80%"></p>
<p align="center"><sub>Inline Site Report panel showing rank, host, country and first-seen date.</sub></p>

<p align="center"><img src="images/netcraft-full-site-report-ip-delegation.png" width="80%"></p>
<p align="center"><sub>Full Site Report: IP delegation chain (IANA → RIR → network owner).</sub></p>

<p align="center"><img src="images/netcraft-trends-site-ranking.png" width="80%"></p>
<p align="center"><sub>Netcraft Trends: historical site ranking data.</sub></p>

## Tools

| Tool | Role |
|---|---|
| Netcraft Browser Extension | Real-time phishing/site reputation detection |
| Netcraft Full Site Report | Network, IP delegation & geolocation intelligence |
| Netcraft Trends | Historical ranking & hosting-change tracking |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to Phishing Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
