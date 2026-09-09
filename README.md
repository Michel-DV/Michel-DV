<p align="center">
  <img src="assets/header.svg" alt="MDV Cybersecurity Portfolio" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/Michel-DV/ProcSentinel-C"><img src="https://img.shields.io/badge/C11-Windows%20Internals-39ff88?style=flat-square&labelColor=111814" alt="C11 Windows Internals" /></a>
  <a href="https://github.com/Michel-DV/Win-TraceGuard"><img src="https://img.shields.io/badge/ETW-Detection%20Engineering-39ff88?style=flat-square&labelColor=111814" alt="ETW Detection Engineering" /></a>
  <a href="https://github.com/Michel-DV/VoidWalker"><img src="https://img.shields.io/badge/Python-IoT%20Security-39ff88?style=flat-square&labelColor=111814" alt="Python IoT Security" /></a>
  <a href="https://github.com/Michel-DV/Go-Fast-Scanner"><img src="https://img.shields.io/badge/Go-Network%20Security-39ff88?style=flat-square&labelColor=111814" alt="Go Network Security" /></a>
  <a href="https://github.com/Michel-DV/Analisi-MyDoom"><img src="https://img.shields.io/badge/YARA%20%2F%20Sigma-Malware%20Analysis-39ff88?style=flat-square&labelColor=111814" alt="Malware Analysis" /></a>
  <a href="https://github.com/Michel-DV/red-ops-security-manual"><img src="https://img.shields.io/badge/RED%20OPS-Field%20Reference-b91c3a?style=flat-square&labelColor=1b0b0f" alt="RED OPS Security Manual" /></a>
</p>

## About this profile

I build practical cybersecurity projects around **Windows internals, endpoint telemetry, detection engineering, malware analysis, network security and IoT security** — and I publish technical field references that turn those ideas into repeatable assessment workflows.

The goal of this profile is not to collect one-off scripts. Each flagship repository is treated as a small engineering project: clear scope, reproducible builds, tests, CI, structured output, documentation and an explicit security boundary.

> **Security scope:** projects here are intended for authorized labs, defensive research, detection engineering, education, or controlled security testing.

## Flagship engineering projects

| Project | What it demonstrates | Stack |
| --- | --- | --- |
| **[ProcSentinel-C](https://github.com/Michel-DV/ProcSentinel-C)** | Windows endpoint and PE triage: process metadata, SHA-256, Authenticode, PE analysis, TCP ownership correlation and explainable risk scoring. | C11 · WinAPI · CMake |
| **[Win-TraceGuard](https://github.com/Michel-DV/Win-TraceGuard)** | ETW telemetry sensor with TDH decoding, PID/PPID correlation, behavioral detections, JSONL capture and replay. | C11 · ETW · TDH · WinAPI |
| **[VoidWalker](https://github.com/Michel-DV/VoidWalker)** | Defensive IoT discovery and exposure triage with SSDP/mDNS evidence, fingerprinting and vulnerability-candidate analysis. | Python · Networking · IoT |
| **[Go-Fast-Scanner](https://github.com/Michel-DV/Go-Fast-Scanner)** | Concurrent TCP connect scanning with bounded workers, cancellation, validated input, IPv4/IPv6-safe addressing and JSON output. | Go · Concurrency · TCP |
| **[Analisi-MyDoom](https://github.com/Michel-DV/Analisi-MyDoom)** | Malware-analysis and detection-engineering case study with report, YARA, Sigma, machine-readable IOCs and ATT&CK mapping. | YARA · Sigma · Python · CTI |
| **[Python-RedTeam-C2-Framework](https://github.com/Michel-DV/Python-RedTeam-C2-Framework)** | Loopback-only controller/agent protocol lab focused on framing, validation, safe command dispatch, testing and detection-oriented study. | Python · Sockets · Protocols |

## Publication & field reference

<a href="https://github.com/Michel-DV/red-ops-security-manual">
  <img src="assets/red-ops-publication.svg" alt="RED OPS Security Manual" width="100%" />
</a>

**[RED OPS Security Manual](https://github.com/Michel-DV/red-ops-security-manual)** is my connected field reference for authorized penetration testing and red team workflows.

The **v1.0.0 Complete Edition** is organized as a 107-page manual with seven complete guides and a 28-page field-card set covering recon, network enumeration, web content discovery, post-exploitation, Active Directory, credential testing, wireless auditing and cross-phase hand-offs.

The public repository is intentionally limited to project information, a controlled preview, provenance records and publication metadata; the complete customer edition and private build/source tree are kept outside the public repo.

Authorship and provenance are explicitly recorded under **Michel-DV** through the repository history, `CITATION.cff`, release manifests, document metadata and copyright notices.

## Legacy Windows research

**[Windows-Process-Injector-C](https://github.com/Michel-DV/Windows-Process-Injector-C)** is intentionally kept outside the flagship engineering set and presented as a **legacy WinAPI research PoC**. It documents the classic `OpenProcess → VirtualAllocEx → WriteProcessMemory → CreateRemoteThread` chain so the underlying Windows primitive can be studied from a malware-analysis and detection-engineering perspective. Its README explicitly documents the technique, defensive telemetry, ATT&CK T1055 mapping, limitations and lab-only scope.

That project is useful in the portfolio because it creates a clear progression:

```text
understand the injection primitive
          ↓
observe endpoint state with ProcSentinel-C
          ↓
correlate behavior over time with Win-TraceGuard
```

## Portfolio map

<p align="center">
  <img src="assets/portfolio-map.svg" alt="MDV security portfolio map" width="100%" />
</p>

## Engineering approach

```text
security idea
    │
    ├── define scope & threat model
    ├── build the smallest useful core
    ├── make behavior observable
    ├── add structured output
    ├── test edge cases
    ├── automate CI
    ├── document assumptions & limits
    └── publish only what has a clear security boundary
```

A few principles recur across the repositories:

- **Explainability over magic scores** — detections and triage signals should show why they fired.
- **Read-only by default** — endpoint tooling favors observation and analysis rather than modification.
- **Safe lab boundaries** — simulation projects are deliberately constrained instead of hiding unrestricted behavior behind a new label.
- **Reproducibility** — CI, tests and build instructions are part of the project, not an afterthought.
- **Useful output** — human-readable terminal views plus JSON/JSONL or machine-readable artifacts where appropriate.
- **Field usability** — documentation should help move from one assessment phase to the next, not just list commands in isolation.

## Project health

<p>
  <a href="https://github.com/Michel-DV/ProcSentinel-C/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/ProcSentinel-C/actions/workflows/ci.yml/badge.svg?branch=main" alt="ProcSentinel-C CI" /></a>
  <a href="https://github.com/Michel-DV/Win-TraceGuard/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/Win-TraceGuard/actions/workflows/ci.yml/badge.svg?branch=main" alt="Win-TraceGuard CI" /></a>
  <a href="https://github.com/Michel-DV/VoidWalker/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/VoidWalker/actions/workflows/ci.yml/badge.svg?branch=main" alt="VoidWalker CI" /></a>
  <a href="https://github.com/Michel-DV/Go-Fast-Scanner/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/Go-Fast-Scanner/actions/workflows/ci.yml/badge.svg?branch=main" alt="Go-Fast-Scanner CI" /></a>
  <a href="https://github.com/Michel-DV/Python-RedTeam-C2-Framework/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/Python-RedTeam-C2-Framework/actions/workflows/ci.yml/badge.svg?branch=main" alt="Python C2 Lab CI" /></a>
  <a href="https://github.com/Michel-DV/Analisi-MyDoom/actions/workflows/build-report.yml"><img src="https://github.com/Michel-DV/Analisi-MyDoom/actions/workflows/build-report.yml/badge.svg?branch=main" alt="MyDoom report CI" /></a>
</p>

## Releases & publications

- **RED OPS Security Manual** — `v1.0.0`
- **ProcSentinel-C** — `v1.0.0`
- **Win-TraceGuard** — `v1.0.1`
- **VoidWalker** — `v2.1.0`
- **Go-Fast-Scanner** — `v2.0.0`
- **Python C2 Lab** — `v2.1.0`
- **MyDoom Analysis & Detection Engineering** — `v2.0.0`

---

<p align="center">
  <sub><code>MDV // build things that make security behavior easier to observe, understand and explain.</code></sub>
</p>
