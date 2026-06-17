---
name: scottbez1__FaderBuddy
source: https://github.com/scottbez1/FaderBuddy/blob/276bdb2ecad74d9952ba961978c376bd63197d22/CLAUDE.md
repo: scottbez1/FaderBuddy
kind: claude-md
stars: 5
last_pushed: 2026-06-08T06:04:55Z
license: apache-2.0
score: 9
domains: [embedded-systems, firmware, iot]
tags: [platformio, i2c, hardware-control, esphome]
curated: 2026-06-15
curated_by: config-scout
---

# scottbez1/FaderBuddy — claude-md

**Why it's worth keeping:** It provides crucial logic-level details (state machines/protocols) alongside exact CLI commands including environment activation requirements, allowing an agent to reason about system behavior rather than just running scripts.

**Summary:** A highly detailed guide covering specialized build workflows for embedded hardware and deep architectural explanations of the I2C protocol.

**Source credibility:** High; well-maintained specialized hardware project with clear documentation and active development.

**Recency:** Current; utilizes modern tooling like PlatformIO, ESPHome, and WebHID.

**Source:** [scottbez1/FaderBuddy/CLAUDE.md](https://github.com/scottbez1/FaderBuddy/blob/276bdb2ecad74d9952ba961978c376bd63197d22/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

FaderBuddy is a bidirectional motor fader control system with integrated capacitive touch sensing and I2C communication. The hardware consists of a PCB that mounts directly onto Soundwell 60mm motorized faders, with an ATtiny1616 microcontroller managing motor control, touch detection, and I2C communication. Multiple faders can be chained together and controlled by an ESP32 host (designed for ESPHome/Home Assistant integration).

## Project Structure

- **electronics/** - KiCad PCB design files (schematic and board layout)
- **firmware/** - ATtiny1616 firmware (PlatformIO project, Arduino framework)
  - `src/main.cpp` - Main firmware logic with motor control loop and I2C peripheral
  - `src/shared/i2c_data.h` - I2C protocol v5 definitions (shared across all components)
- **esphome/** - ESPHome custom component for Home Assistant integration
  - `components/fader_buddy/` - Core component for interfacing with FaderBuddy boards
  - `examples/multi-fader-display.yaml` - ESP32-S3 example with LVGL display
- **software/** - Software tools and demos
  -
```

</details>
