<p align="center">
  <img src="assets/header.svg" alt="MDV Cybersecurity Portfolio" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/Michel-DV/ProcSentinel-C"><img src="https://img.shields.io/badge/C11-Windows%20Internals-39ff88?style=flat-square&labelColor=111814" alt="C11 Windows Internals" /></a>
  <a href="https://github.com/Michel-DV/Win-TraceGuard"><img src="https://img.shields.io/badge/ETW-Detection%20Engineering-39ff88?style=flat-square&labelColor=111814" alt="ETW Detection Engineering" /></a>
  <a href="https://github.com/Michel-DV/VoidWalker"><img src="https://img.shields.io/badge/Python-IoT%20Security-39ff88?style=flat-square&labelColor=111814" alt="Python IoT Security" /></a>
  <a href="https://github.com/Michel-DV/Go-Fast-Scanner"><img src="https://img.shields.io/badge/Go-Network%20Security-39ff88?style=flat-square&labelColor=111814" alt="Go Network Security" /></a>
  <a href="https://github.com/Michel-DV/Analisi-MyDoom"><img src="https://img.shields.io/badge/YARA%20%2F%20Sigma-Malware%20Analysis-39ff88?style=flat-square&labelColor=111814" alt="Malware Analysis" /></a>
</p>

## About this profile

I build practical cybersecurity projects around **Windows internals, endpoint telemetry, detection engineering, malware analysis, network security and IoT security**.

The goal of this profile is not to collect one-off scripts. Each flagship repository is treated as a small engineering project: clear scope, reproducible builds, tests, CI, structured output, documentation and an explicit security boundary.

> **Security scope:** projects here are intended for authorized labs, defensive research, detection engineering, education, or controlled security testing.

## Flagship projects

| Project | What it demonstrates | Stack |
| --- | --- | --- |
| **[ProcSentinel-C](https://github.com/Michel-DV/ProcSentinel-C)** | Windows endpoint and PE triage: process metadata, SHA-256, Authenticode, PE analysis, TCP ownership correlation and explainable risk scoring. | C11 · WinAPI · CMake |
| **[Win-TraceGuard](https://github.com/Michel-DV/Win-TraceGuard)** | ETW telemetry sensor with TDH decoding, PID/PPID correlation, behavioral detections, JSONL capture and replay. | C11 · ETW · TDH · WinAPI |
| **[VoidWalker](https://github.com/Michel-DV/VoidWalker)** | Defensive IoT discovery and exposure triage with SSDP/mDNS evidence, fingerprinting and vulnerability-candidate analysis. | Python · Networking · IoT |
| **[Go-Fast-Scanner](https://github.com/Michel-DV/Go-Fast-Scanner)** | Concurrent TCP connect scanning with bounded workers, cancellation, validated input, IPv4/IPv6-safe addressing and JSON output. | Go · Concurrency · TCP |
| **[Analisi-MyDoom](https://github.com/Michel-DV/Analisi-MyDoom)** | Malware-analysis and detection-engineering case study with report, YARA, Sigma, machine-readable IOCs and ATT&CK mapping. | YARA · Sigma · Python · CTI |
| **[Python-RedTeam-C2-Framework](https://github.com/Michel-DV/Python-RedTeam-C2-Framework)** | Loopback-only controller/agent protocol lab focused on framing, validation, safe command dispatch, testing and detection-oriented study. | Python · Sockets · Protocols |

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
    └── document assumptions, limits & security boundaries
```

A few principles recur across the repositories:

- **Explainability over magic scores** — detections and triage signals should show why they fired.
- **Read-only by default** — endpoint tooling favors observation and analysis rather than modification.
- **Safe lab boundaries** — simulation projects are deliberately constrained instead of hiding unrestricted behavior behind a new label.
- **Reproducibility** — CI, tests and build instructions are part of the project, not an afterthought.
- **Useful output** — human-readable terminal views plus JSON/JSONL or machine-readable artifacts where appropriate.

## Project health

<p>
  <a href="https://github.com/Michel-DV/ProcSentinel-C/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/ProcSentinel-C/actions/workflows/ci.yml/badge.svg?branch=main" alt="ProcSentinel-C CI" /></a>
  <a href="https://github.com/Michel-DV/Win-TraceGuard/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/Win-TraceGuard/actions/workflows/ci.yml/badge.svg?branch=main" alt="Win-TraceGuard CI" /></a>
  <a href="https://github.com/Michel-DV/VoidWalker/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/VoidWalker/actions/workflows/ci.yml/badge.svg?branch=main" alt="VoidWalker CI" /></a>
  <a href="https://github.com/Michel-DV/Go-Fast-Scanner/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/Go-Fast-Scanner/actions/workflows/ci.yml/badge.svg?branch=main" alt="Go-Fast-Scanner CI" /></a>
  <a href="https://github.com/Michel-DV/Python-RedTeam-C2-Framework/actions/workflows/ci.yml"><img src="https://github.com/Michel-DV/Python-RedTeam-C2-Framework/actions/workflows/ci.yml/badge.svg?branch=main" alt="Python C2 Lab CI" /></a>
  <a href="https://github.com/Michel-DV/Analisi-MyDoom/actions/workflows/build-report.yml"><img src="https://github.com/Michel-DV/Analisi-MyDoom/actions/workflows/build-report.yml/badge.svg?branch=main" alt="MyDoom report CI" /></a>
</p>

## Releases

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
