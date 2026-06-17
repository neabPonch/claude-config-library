---
name: CharlieNance__puff-trigger
source: https://github.com/CharlieNance/puff-trigger/blob/18b616315bdee9acd0b2e2f6ea5743a694eb49a8/claude.md
repo: CharlieNance/puff-trigger
kind: claude-md
stars: 0
last_pushed: 2026-04-17T01:17:19Z
license: mit
score: 9
domains: [embedded-systems, iot, hardware-integration]
tags: [raspberry-pi, mocking, cross-platform, sensor-data]
curated: 2026-06-15
curated_by: config-scout
---

# CharlieNance/puff-trigger — claude-md

**Why it's worth keeping:** Provides exceptional instructions on the interface/mock pattern for hardware abstraction, explicit hardware resource constraints (RAM/CPU), and environment-specific dependency management.

**Summary:** A specialized hardware-software integration guide for a Raspberry Pi project that manages the gap between Windows development and Pi deployment.

**Source credibility:** A highly specific personal project with recent activity and detailed technical specifications.

**Recency:** Very current; utilizes modern stacks like FastAPI, Svelte, and Python 3.11.

**Source:** [CharlieNance/puff-trigger/claude.md](https://github.com/CharlieNance/puff-trigger/blob/18b616315bdee9acd0b2e2f6ea5743a694eb49a8/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Puff Trigger — Claude Context

## Project Overview

Puff Trigger is a Raspberry Pi Zero W project that detects air quality changes (specifically particulate matter spikes from blowing smoke at the sensor) and triggers audio playback through a connected USB speaker. Phase 1 plays the "It's John Cena!" audio clip. Long-term goal: a Smokey the Bear-themed 3D-printed enclosure.

## Hardware

| Component | Details |
|---|---|
| Raspberry Pi Zero W | hostname `chuck-local-pi.local`, SSH via ED25519 key |
| Pimoroni PIM458 Enviro+ HAT | seated on GPIO; I2C verified (BH1750, ADS1015, BME280 detected) |
| PMS5003 Particulate Sensor | connected to Enviro+ HAT; UART via `/dev/ttyS0` |
| USB Speaker | Jieli UACDemoV1.0; ALSA card 1; volume 75%, persisted via `alsactl store` |
| Powered USB Hub | Huasheng 3-port; required since Zero W OTG can't power the speaker alone |

The `enviroplus` library is installed from PyPI (not git clone). System deps (`python3-smbus`, `i2c-tools`, `libgpiod-dev`) must be installed separately on the Pi.

## Architecture

The Pi Zero W (512MB RAM, 1GHz single-core) cannot run a frontend dev server alongside the backend. The system is split:

- **Pi Zero W:** FastAP
```

</details>
