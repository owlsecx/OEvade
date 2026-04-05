# 🛡️ OEvade

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ORec%20%2F%20Adversary%20Simulation-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(stdlib)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **OEvade** is a purple team evasion simulator that safely demonstrates advanced evasion techniques to test EDR behavioral detection, analytics, and blue team response. All techniques are **non-destructive simulations only**.

**Perfect for purple team exercises and improving detection rules.**

---

## 📌 Overview

OEvade simulates real-world adversary evasion techniques without executing any actual malicious code. It covers AMSI bypass, ETW tampering, obfuscation, C2 beaconing, sleep masking, indirect syscalls, and process injection — each with realistic output and MITRE ATT&CK mapping.

Designed to help blue teams tune their detection and response.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **AMSI Bypass**         | T1562.001 — AMSI scan buffer patching & obfuscated PowerShell |
| **[2]** | **ETW Tampering**       | T1562.006 — Event Tracing for Windows suppression |
| **[3]** | **Obfuscation**         | T1027     — Multi-layer command obfuscation |
| **[4]** | **C2 Beaconing**        | T1071/T1573 — Encrypted jittered beacon simulation |
| **[5]** | **Sleep Masking**       | T1497.003 — Chunked/jittered sleep evasion |
| **[6]** | **Indirect Syscalls**   | T1055.004 — NT syscall resolution & indirect calls |
| **[7]** | **Process Injection**   | T1055     — Simulated injection chains |
| **[8]** | **Full Evasion Chain**  | Runs all 7 techniques sequentially |

---

## 📊 Key Features

- **7 Realistic Evasion Techniques** — Each mapped to MITRE ATT&CK
- **Non-Destructive** — No real payloads, no memory writes, no process injection
- **Live Simulation Output** — Colored progress, realistic logs, and detection guidance
- **Event Logging** — Full simulation timeline saved to report
- **C2 Beacon Simulation** — Safe loopback connection with jitter
- **Sleep Masking** — Visual chunked delay with progress bar
- **Report Generation** — Detailed TXT report with MITRE guidance
- **Pure stdlib** — No external dependencies

---

## ⚙️ Requirements

- **No dependencies** — Uses only Python standard library
- **Run as normal user** — No root required (all simulations are safe)

**Standalone executable** — Runs as `./OEvade` when built with PyInstaller.

---

## 🚀 Usage

```bash
./OEvade

📁 Output

Live Terminal — Colored simulation steps, technique details, and detection guidance
Event Log — Timestamped simulation events with technique, action, and result
Report File (in oevade_reports/):
oevade_YYYYMMDD_HHMMSS.txt — Full timeline + MITRE ATT&CK guidance for blue team



📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED PURPLE TEAM USE ONLY
Run ONLY in environments you own or have written permission.
