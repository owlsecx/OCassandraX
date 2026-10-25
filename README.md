# 🦉 OCassandraX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OCassandraX** — Offline NoSQL Wide-Column / Document Store

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OCassandraX is an offline, read-only configuration auditor for NoSQL wide-column and document stores, covering Cassandra, ScyllaDB, CouchDB and Memcached. Stdlib YAML-lite and INI parsers with file:line origins drive checks for weak authentication, missing TLS, dangerous exposure, UDF RCE and known CVEs. Findings map to CWE/CVE/MITRE ATT&CK with hardened templates, a score and an A+…F grade.

---

## ✨ Features

- Cassandra/ScyllaDB: AllowAll auth, 0.0.0.0 binds, TLS, UDF RCE (CVE-2021-44521), JMX
- CouchDB: admin party, weak admins, CORS *, TLS and 'monster' cookie CVEs
- Memcached: 0.0.0.0 listeners, UDP amplification, SASL and run-as-root checks
- Stdlib YAML-lite/INI parsers with file:line origin and offline --root discovery
- CWE / CVE / MITRE ATT&CK mapping with secrets masked
- Hardened templates, scoring/grade and export TXT/MD/JSON/CSV/SARIF

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCassandraX --scan
./OCassandraX --cassandra cassandra.yaml --format sarif -o report.sarif --fail-on high
./OCassandraX --couchdb /etc/couchdb/local.ini
./OCassandraX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
