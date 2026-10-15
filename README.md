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

Offline Cassandra / ScyllaDB / CouchDB / Memcached configuration auditor

---

## ✨ Features

- Stdlib YAML-lite + INI parsers with file:line origin
- Cassandra / ScyllaDB — AllowAll auth, Transitional auth, rpc/listen 0.0.0.0, Thrift, client & internode TLS, default keystore passwords, UDF RCE (CVE-2021-44521), audit logging, CDC, /tmp data dirs
- cassandra-env.sh JMX (LOCAL_JMX=no w/o auth / SSL), cqlshrc default cassandra/cassandra superuser
- Scylla Alternator w/o authorization, REST API, dev mode
- CouchDB INI stack — admin party, plaintext / SHA-1 admins, require_valid_user, CORS *, TLS, cookies, CVE-2017-12635/12636, CVE-2022-24706 'monster' cookie
- Memcached — -l 0.0.0.0, UDP (CVE-2018-1000115), SASL, -u root, -A, TLS (Debian / sysconfig / systemd)
- Offline --root discovery, CWE / CVE / MITRE mapping
- Export TXT / MD / JSON / CSV / SARIF, --demo, CI gates

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCassandraX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
