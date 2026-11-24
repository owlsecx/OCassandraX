# 🦉 OCassandraX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
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

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*

---

## 🔍 Verification & Transparency

This tool is closed-source. These files let you see exactly what is inside it,
without the source:

- [`SBOM.cdx.json`](SBOM.cdx.json) — CycloneDX inventory: SHA-256 of this
  binary, bundled CPython version, and every bundled library with its exact
  version and license. Feed it to Grype, Trivy or Dependency-Track to audit
  our dependencies for CVEs yourself.
- [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) — the full license text
  of every third-party component, extracted from this binary.

**No telemetry, no analytics, no licence check-in.** This tool does not phone
home. Verify that claim yourself:

```bash
sudo strace -f -e trace=network ./OCassandraX --help   # watch every network call
firejail --net=none ./OCassandraX --help               # deny the network entirely
```

Release signing, GPL compliance and vulnerability reporting:
[**TRUST.md**](https://github.com/owlsecx/owl-os/blob/main/TRUST.md)
