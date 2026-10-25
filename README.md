# 🦉 OIpaX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OCore-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OIpaX** — FreeIPA / Red Hat IdM Server Configuration Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OIpaX — FreeIPA / Red Hat IdM Server Configuration Auditor. It provides offline, read-only IdM *server* audit — never talks to LDAP / Kerberos / HTTP, never runs `ipa`, never writes; Parsers: `ipa … --all` text, LDIF, CS.cfg / profiles, default.conf, httpd conf.d; --root image discovery. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- Offline, read-only IdM *server* audit — never talks to LDAP / Kerberos / HTTP, never runs `ipa`, never writes
- Parsers: `ipa … --all` text, LDIF, CS.cfg / profiles, default.conf, httpd conf.d; --root image discovery
- HBAC, sudo, password policy, ipa config, users / 2FA, services, 389-DS, replication, Dogtag, httpd, DNS, CA / RA / KDC key and PIN permissions — 110+ rules
- Secrets masked; CWE + MITRE ATT&CK; A+…F grading
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Self-test --demo, CI gates --fail-on / --min-severity

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OIpaX                                     # interactive menu
./OIpaX --scan -r /path/to/root
./OIpaX --demo
./OIpaX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
