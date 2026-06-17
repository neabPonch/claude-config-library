---
name: greystoke1337__localized-air-traffic-tracker
source: https://github.com/greystoke1337/localized-air-traffic-tracker/blob/95852d64ab5293e06fddf57dcb15fe37351b1b43/CLAUDE.md
repo: greystoke1337/localized-air-traffic-tracker
kind: claude-md
stars: 26
last_pushed: 2026-04-21T01:15:14Z
license: unknown
score: 9
domains: [iot, embedded-systems, fullstack-web, agentic-workflows]
tags: [iot, hardware, multi-component, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# greystoke1337/localized-air-traffic-tracker — claude-md

**Why it's worth keeping:** Uses high-density information tables for component/tech mapping and introduces 'Specialist Agents' to direct Claude toward domain-specific files. It also effectively communicates strict architectural constraints like the 'no-build' rule.

**Summary:** A comprehensive architectural blueprint for a distributed IoT and web ecosystem, mapping hardware components to their specific technical implementations.

**Source credibility:** High; contains deep technical specifics (pinouts, hardware models, deployment routes) consistent with a real project.

**Recency:** Current; optimized for agentic workflows and modern CLI-based development.

**Source:** [greystoke1337/localized-air-traffic-tracker/CLAUDE.md](https://github.com/greystoke1337/localized-air-traffic-tracker/blob/95852d64ab5293e06fddf57dcb15fe37351b1b43/CLAUDE.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions

## Project Overview

**Overhead Tracker** is a real-time aircraft tracking system.
It answers: *"What planes are flying directly above me right now?"*

Five components:

| Component | Codename | Tech | Hosted at |
|-----------|----------|------|-----------|
| Web app | — | Single-file HTML + vanilla JS | GitHub Pages (auto-deploy on push to `master`) |
| Proxy server | — | Node.js / Express | Railway (`api.overheadtracker.com`) |
| ESP32 firmware (4.0") | **Echo** | Arduino C++ on Freenove FNK0103S | Physical device (USB via `build.sh`, COM4) |
| ESP32-S3 firmware (4.3") | **Foxtrot** | Arduino C++ on Waveshare ESP32-S3-Touch-LCD-4.3 | Physical device (USB via `arduino-cli`, COM7) |
| ESP32-S3 firmware (3.49") | **Delta** | Arduino C++ on Waveshare ESP32-S3-Touch-LCD-3.49 | Physical device (USB via `build.sh delta`, COM8) |
| Pi display | — | Python / Pygame on Raspberry Pi 3B+ | Physical device (3.5" TFT on `/dev/fb0`, systemd `tft-display.service`) |
| 64×32 LED matrix | **Golf** | Arduino C++ on Adafruit Matrix Portal M4 | Physical device (USB via `build.sh golf`, COM9) |

Live URL: https://greystoke1337.github.io/localized-air-traffic-tracker/
Custom
```

</details>
