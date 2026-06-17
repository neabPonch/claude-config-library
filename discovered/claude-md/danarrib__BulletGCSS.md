---
name: danarrib__BulletGCSS
source: https://github.com/danarrib/BulletGCSS/blob/fcbfd43057b0b4e4c1d24e6d5b1604d8f7325aa8/CLAUDE.md
repo: danarrib/BulletGCSS
kind: claude-md
stars: 58
last_pushed: 2026-04-21T02:24:14Z
license: gpl-3.0
score: 9
domains: [embedded-firmware, iot, web-pwa]
tags: [msp-protocol, esp32, hardware-interfacing, system-state]
curated: 2026-06-14
curated_by: config-scout
---

# danarrib/BulletGCSS — claude-md

**Why it's worth keeping:** Includes explicit execution sequences (e.g., startup protocols), specific debugging workflows for hardware serial ports, and 'injection' commands to simulate UI states via the browser console.

**Summary:** Detailed technical manual for a dual-component (ESP32/Web) system that emphasizes protocol logic and state manipulation.

**Source credibility:** Niche drone project with moderate engagement and recent activity.

**Recency:** Highly relevant; provides the exact type of execution-flow detail that helps LLMs reason about side effects.

**Source:** [danarrib/BulletGCSS/CLAUDE.md](https://github.com/danarrib/BulletGCSS/blob/fcbfd43057b0b4e4c1d24e6d5b1604d8f7325aa8/CLAUDE.md) · 58★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Bullet GCSS** (Ground Control Station System) is a web-based UAV ground control station that operates over cellular networks with no range limit. It is a PWA (no app installation required) that works cross-platform.

## Two-Component Architecture

### 1. ESP32-Modem (Embedded Firmware — [ESP32-Modem/](ESP32-Modem/))
Runs on an ESP32 board aboard the UAV. Communicates with the flight controller via the **MSP v2 protocol** (UART, 115200 baud on Serial2: TX18/RX19), then publishes telemetry as key:value messages to an **MQTT broker** via WiFi or a cellular modem (SIM800/SIM7600).

- [ESP32-Modem.cpp](ESP32-Modem/ESP32-Modem.cpp): Main source file. Runs two tasks: `fcTask` (FreeRTOS, priority 2, Core 1 — all MSP, ticks every 160 ms via `TASK_MSP_READ_MS`) and the Arduino loop task (MQTT publish, every 1000 ms). Key startup sequence on FC connection: `msp_get_boxnames()` → `msp_get_mode_ranges()` → `msp_get_override_channels()`. Per-cycle (every 160 ms): `msp_get_rc()` + `msp_send_rc_override()`. Telemetry split into 6 round-robin groups (one per cy
```

</details>
