---
name: laurigates__mcu-tinkering-lab
source: https://github.com/laurigates/mcu-tinkering-lab/blob/3b6aa1ad23141b679ebda9448c1ca56cea0c80ef/CLAUDE.md
repo: laurigates/mcu-tinkering-lab
kind: claude-md
stars: 6
last_pushed: 2026-06-12T16:53:52Z
license: mit
score: 9
domains: [embedded-systems, iot, monorepo]
tags: [esp32, cmake, firmware, justfile]
curated: 2026-06-15
curated_by: config-scout
---

# laurigates/mcu-tinkering-lab — claude-md

**Why it's worth keeping:** It utilizes structured command tables for developer workflows and includes critical hardware-level constraints (GPIO/UART) that prevent AI-generated errors in firmware logic.

**Summary:** A comprehensive technical manual for an embedded systems monorepo that provides highly specific navigation, build, and architectural context.

**Source credibility:** Strong; the repository is active with recent commits and a well-defined specialized domain.

**Recency:** Very current, leveraging modern tooling like 'uv', 'ruff', and latest ESP-IDF versions.

**Source:** [laurigates/mcu-tinkering-lab/CLAUDE.md](https://github.com/laurigates/mcu-tinkering-lab/blob/3b6aa1ad23141b679ebda9448c1ca56cea0c80ef/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

MCU Tinkering Lab is a production-ready embedded systems monorepo for ESP32, STM32, and Arduino platforms. The primary project is an AI-powered dual-ESP32 robot car with computer vision.

## Repository Structure

Projects are grouped by domain under `packages/`. Add new projects to the
folder that matches the domain, or create a new domain folder. Drop the
`esp32-` prefix — the category already implies it.

```
mcu-tinkering-lab/
├── packages/
│   ├── robocar/                    # Dual-ESP32 AI robot car system
│   │   ├── main/                   # Main controller (Heltec WiFi LoRa 32)
│   │   ├── camera/                 # ESP32-CAM vision (Claude/Ollama/Gemini)
│   │   ├── unified/                # Single-board XIAO ESP32-S3 Sense consolidation
│   │   ├── simulation/             # Python 3.11 physics simulation (Pymunk)
│   │   ├── docs/                   # Docs and coordination justfile
│   │   └── components/i2c-protocol/ # Robocar-internal I2C protocol + tests
│   ├── camera-vision/              # Standalone camera / AI vision projects
│
```

</details>
