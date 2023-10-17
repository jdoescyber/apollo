---
footer: "TLP: CLEAR"
title: Malcat Overview
date: 2023-09
---

# **Malcat**

Quick and Efficient Binary Analysis Software

![](https://malcat.fr/theme/images/malcat.png)

## BLUF

- Quick analysis of suspicious files (incl. Office docs, PDFs, executables, and more)
- FireEye's [Capa](https://github.com/mandiant/capa) built in
- [Yara](https://virustotal.github.io/yara/) rule matching
- No reliance on web APIs (e.g. VT)
    - Available but costs `$$`/yr

## Features

![[_attachments/features.png]]

- Most core features available for free in the "lite" edition
- Left to right: "Lite," "MalCat," "MalCat Pro"

## Why?

- Dynamic analysis can be time consuming, static analysis **very** time consuming
- Lots of common static analysis tasks get completed very quickly w/ MalCat
- Make a determination if more analysis is needed
    - "Does this Defender detection have any merit or is it another FP?"
- Limited (or no) OPSEC concerns compared to public services

## Example: CobaltStrike 

- Sample available on [Malware Bazaar](https://bazaar.abuse.ch/sample/a92a6d6f59fd04e04c6f911e39219c61eb6013e6db92905796642092dc1ce3d7/)
- 43 Yara rules matched by the sample
- Cape Sandbox results [here](https://www.capesandbox.com/analysis/433330/)

![[_attachments/cstrike-overview.png]]

## Yara Results

![[_attachments/cstrike-yara.png]]