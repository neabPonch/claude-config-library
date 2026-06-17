---
name: jontiritilli__life-puck
source: https://github.com/jontiritilli/life-puck/blob/e958d8b890c6242108f4c243e747406147ad2f73/CLAUDE.md
repo: jontiritilli/life-puck
kind: claude-md
stars: 19
last_pushed: 2025-11-06T01:19:11Z
license: other
score: 9
domains: [embedded-systems, firmware]
tags: [esp32, arduino, hardware-abstraction, lvgl]
curated: 2026-06-15
curated_by: config-scout
---

# jontiritilli/life-puck — claude-md

**Why it's worth keeping:** Includes crucial 'Order Matters' sequences and version-specific API warnings (LVGL v9) that prevent the AI from introducing breaking changes in specialized environments.

**Summary:** Provides exhaustive technical context for an ESP32 embedded project, including hardware initialization order and specific board variants.

**Source credibility:** A legitimate hobbyist/specialized hardware project with a decent star count for its niche.

**Recency:** 

**Source:** [jontiritilli/life-puck/CLAUDE.md](https://github.com/jontiritilli/life-puck/blob/e958d8b890c6242108f4c243e747406147ad2f73/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Life Puck** is an embedded firmware project for ESP32-S3 devices that provides a digital life counter for Magic: The Gathering, Yu-Gi-Oh!, Pokémon TCG, and other tabletop card games. It runs on Waveshare ESP32-S3 round display modules (1.85" LCD, 360x360px) with capacitive touch screens.

### Key Technologies
- **Platform:** ESP32-S3 (16MB Flash, 8MB PSRAM)
- **Framework:** Arduino 3.x (ESP-IDF 5.3 via pioarduino)
- **Display:** ST77916 driver (QSPI mode), 1.85" round LCD
- **Touch:** CST816 capacitive touch controller
- **GUI:** LVGL 9.3.0
- **Storage:** NVS (Non-Volatile Storage) for persistent settings

## Build Commands

### Build the project
```bash
pio run
```

### Upload to device
```bash
pio run -t upload
```

### Build and upload in one step
```bash
pio run -t upload && pio device monitor
```

### Serial monitor (115200 baud)
```bash
pio device monitor
```

### Clean build
```bash
pio run -t clean && pio run
```

### Erase flash completely
```bash
pio run -t erase
```

### Switch between board variants
Edit `platformio.ini` and change
```

</details>
