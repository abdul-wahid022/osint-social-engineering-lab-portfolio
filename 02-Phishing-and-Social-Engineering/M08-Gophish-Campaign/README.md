<p align="center">
  <img src="images/cover.png" alt="Gophish Campaign Cover" width="100%">
</p>

<h1 align="center">Phishing Simulation & Campaign Tracking (Gophish)</h1>
<h3 align="center">End-to-End Phishing Campaign Lifecycle — Setup to Delivery Tracking</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Module-M08-red?style=flat-square" alt="Module">
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
| Objective | Build and launch a complete phishing campaign using Gophish, from sending profile to delivery tracking |
| Platform | Kali Linux, Gophish v0.12.1 |
| Components | Sending Profile, Landing Page, Email Template, Users & Groups, Campaign |

## Key Findings

| Component | Status |
|---|---|
| Sending Profile (Gmail SMTP + App Password) | ✅ Configured and test email delivered |
| Landing Page | ✅ Cloned test page with credential capture + redirect enabled |
| Email Template | ✅ Imported branded email (tracking pixel + link rewriting enabled) |
| Users & Groups | ✅ 3 test recipients added |
| Campaign Launch | ✅ Scheduled and launched |
| Delivery Result | ⚠ 2 recipients showed Error status (recipient-side filtering, not a Gophish fault) |

## Evidence

<p align="center"><img src="images/gophish-sending-profile-configured.png" width="80%"></p>
<p align="center"><sub>Sending Profile configured with SMTP host and sender address.</sub></p>

<p align="center"><img src="images/gophish-test-email-sent-confirmation.png" width="80%"></p>
<p align="center"><sub>"Email Sent!" confirmation after test email dispatch.</sub></p>

<p align="center"><img src="images/gophish-landing-page-credential-capture.png" width="80%"></p>
<p align="center"><sub>Landing page with Capture Submitted Data/Passwords and redirect enabled.</sub></p>

<p align="center"><img src="images/gophish-campaign-results-details-table.png" width="80%"></p>
<p align="center"><sub>Campaign details table showing per-recipient delivery status.</sub></p>

## Tools

| Tool | Role |
|---|---|
| Gophish | Phishing campaign dashboard — profiles, templates, landing pages, tracking |
| Gmail SMTP + App Password | Authenticated email delivery |
| Bitly | Campaign URL shortening |

---

<p align="center">
  <a href="Lab-Report.pdf">📄 Full Report</a> ·
  <a href="../README.md">⬅ Back to Phishing Section</a> ·
  <a href="../../README.md">⬅ Back to Main Repo</a>
</p>
