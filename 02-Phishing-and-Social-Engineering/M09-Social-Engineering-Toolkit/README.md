<p align="center">
  <img src="images/cover.png" alt="Social Engineering Toolkit Cover" width="100%">
</p>

<h1 align="center">Social Engineering & Phishing Simulation (SET)</h1>
<h3 align="center">Payload Delivery, Mass Mailer, and Credential Harvesting</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M09-red?style=flat-square" alt="Module">
  <img src="https://img.shields.io/badge/Category-Phishing-critical?style=flat-square" alt="Category">
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
| Objective | Simulate payload-based phishing (Mass Mailer) and credential harvesting with the Social-Engineer Toolkit |
| Platform | Kali Linux, SET v8.0.3 ("Maverick") |
| Attack Chains | Mass Mailer Attack (payload + listener), Credential Harvester, Site Cloner + link spoofing |

## Key Findings

| Module | Status | Notes |
|---|---|---|
| Payload Generation | ✅ Success | Windows Reverse TCP Meterpreter payload generated |
| Netcat Listener | ✅ Success | Listener active on port 4444 |
| Link Shortening | ✅ Success | Payload URL shortened via Bitly |
| Mass Mailer Delivery | ⚠ Auth Error | Gmail SMTP App Password misconfiguration — not a SET flaw |
| Credential Harvester | ✅ Success | Test credentials captured in cleartext from a cloned login page |
| Site Cloner + Link Spoofing | ✅ Success | Victim redirected via a trusted-looking Gmail link to the cloned page |

## Evidence

<p align="center"><img src="images/set-main-menu-interface.png" width="80%"></p>
<p align="center"><sub>SET main menu after accepting terms of service.</sub></p>

<p align="center"><img src="images/set-payload-generation-lhost-lport.png" width="80%"></p>
<p align="center"><sub>Payload generation with LHOST/LPORT configuration.</sub></p>

<p align="center"><img src="images/netcat-listener-active-port-4444.png" width="80%"></p>
<p align="center"><sub>Netcat listener active on port 4444, awaiting connection.</sub></p>

<p align="center"><img src="images/set-credential-harvester-terminal-capture.png" width="80%"></p>
<p align="center"><sub>SET terminal confirming captured username/password fields (test credentials only).</sub></p>

## Tools

| Tool | Role |
|---|---|
| Social-Engineer Toolkit (SET) | Mass mailer, credential harvester, site cloner |
| Metasploit Framework | Reverse TCP Meterpreter payload & listener |
| Netcat | Manual reverse-shell listener |
| Bitly | Payload URL shortening |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to Phishing Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
