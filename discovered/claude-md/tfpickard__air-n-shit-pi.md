---
name: tfpickard__air-n-shit-pi
source: https://github.com/tfpickard/air-n-shit-pi/blob/ba5cc86734cfbfa308e3b202f5b3835c64378b38/CLAUDE.MD
repo: tfpickard/air-n-shit-pi
kind: claude-md
stars: 0
last_pushed: 2025-12-19T00:34:56Z
license: mpl-2.0
score: 8
domains: [iot, embedded-systems, fullstack]
tags: [architecture-diagram, hardware-specification, system-blueprint]
curated: 2026-06-15
curated_by: config-scout
---

# tfpickard/air-n-shit-pi — claude-md

**Why it's worth keeping:** The ASCII architecture diagram provides essential spatial context for data flow, while the explicit I2C/sensor mappings prevent hallucinations during driver implementation. The inclusion of strict 'Staff-level' quality constraints sets clear expectations for error handling and production readiness.

**Summary:** This file acts as a high-fidelity system blueprint combining architectural diagrams, hardware specifications, and directory maps. It transforms the LLM from a generic coder into a domain-aware engineer for this specific IoT ecosystem.

**Source credibility:** Low social proof (0 stars), but extremely high technical depth in documentation suggests a highly competent author.

**Recency:** Extremely current, referencing bleeding-edge software like Python 3.14 and Ubuntu 25.04.

**Source:** [tfpickard/air-n-shit-pi/CLAUDE.MD](https://github.com/tfpickard/air-n-shit-pi/blob/ba5cc86734cfbfa308e3b202f5b3835c64378b38/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Air Quality & IoT Monitoring System - Project Specification

## Project Overview

A production-ready, secure IoT monitoring system running on Raspberry Pi 4 (edge) with a Next.js dashboard (cloud on Vercel). This is **NOT** a proof-of-concept. All code must be production-quality with proper error handling, security, testing, and observability.

**Project Name**: air-n-shit-pi
**Architecture**: Distributed edge + cloud monorepo
**Quality Standard**: Staff-level engineering with no placeholders or TODOs for core features

---

## System Architecture (ASCII)

```
┌─────────────────────────────────────────────────────────────┐
│                     RASPBERRY PI 4 (Edge)                   │
│  ┌────────────────────────────────────────────────────────┐ │
│  │  Hardware Layer                                         │ │
│  │  • SCD40 (CO₂, Temp, Humidity) ─────┐                  │ │
│  │  • SGP40 (VOC/IAQ)          ────────┤─── I2C Bus       │ │
│  │  • Presence Sensor          ────────┤                  │ │
│  │  • SparkFun QuickFAT (Storage) ─────┘                  │ │
│  │  • GPS Module (USB/Serial NMEA)                        │ │
│  │  • Cellular Modem (USB/Network)
```

</details>
