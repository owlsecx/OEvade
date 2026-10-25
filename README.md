# 🦉 OEvade

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OAttack%20/%20Offensive-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OEvade** — EDR Evasion Technique Detection Tester

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OEvade simulates EDR evasion technique indicators so blue teams can validate behavioural detections. It is non-destructive and distinct from OCymulate (C2 BAS) and related OwlSec purple-team tools. Default targeting stays local/safe, with explicit opt-ins for live simulation and external hosts.

---

## ✨ Features

- Catalogue of evasion technique indicators runnable by key
- List mode to inventory available techniques
- Dry-run versus live-sim controls for detection drills
- Beacon host/port/count and sleep-masking duration parameters
- Text/JSON reports and optional detection gap reporting
- Unsafe-external gate for authorised off-box simulation

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OEvade --list
./OEvade --run 1 --dry-run
./OEvade --run A --host 127.0.0.1 --port 4444 --count 3 --json
./OEvade --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
