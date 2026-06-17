---
name: opivankristovi__udoo-key-arduino
source: https://github.com/opivankristovi/udoo-key-arduino/blob/a95ebef2fad4c6adf96d160fb760a52d297b2f46/CLAUDE.md
repo: opivankristovi/udoo-key-arduino
kind: claude-md
stars: 10
last_pushed: 2026-04-29T19:05:24Z
license: unknown
score: 9
domains: [embedded-systems, iot]
tags: [slash-commands, scaffolding, hardware-mapping, dual-mcu]
curated: 2026-06-16
curated_by: config-scout
---

# opivankristovi/udoo-key-arduino — claude-md

**Why it's worth keeping:** Demonstrates the advanced technique of using project-specific slash commands to automate multi-directory boilerplate; provides structured pinout tables as ground truth for high-accuracy embedded coding.

**Summary:** Provides a hardware-centric reference and defines custom slash commands to scaffold complex dual-MCU code structures.

**Source credibility:** A niche hardware repository with moderate social proof (10 stars).

**Recency:** Extremely current, specifically targeting the Claude Code ecosystem.

**Source:** [opivankristovi/udoo-key-arduino/CLAUDE.md](https://github.com/opivankristovi/udoo-key-arduino/blob/a95ebef2fad4c6adf96d160fb760a52d297b2f46/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Udoo Key Arduino Repository

## Board overview

The **Udoo Key** is a dual-MCU development board:
- **ESP32** — handles Wi-Fi, Bluetooth, I2S microphone (Pro), IMU/MPU6500 (Pro), and on-board UART to RP2040
- **RP2040** — general GPIO, sensors, and on-board UART to ESP32

The **Udoo Key Pro** adds an on-board SPK0838HT4H-1 I2S digital microphone (wired to the ESP32) and an MPU-6500 6-axis IMU. The IMU is physically connected to **both** MCUs; a 3-pin jumper selects which one can talk to it over I2C (default: ESP32 — no jumper placed).

## Repository structure

```
esp32/      — sketches to be flashed to the ESP32
rp2040/     — sketches to be flashed to the RP2040
REFERENCE.md — quick-reference pinout tables
```

## Arduino IDE board selection

| MCU   | Board to select in Arduino IDE |
|-------|-------------------------------|
| ESP32 | ESP32 Dev Module               |
| RP2040 | Raspberry Pi Pico Module      |

Board manager URLs (add under File → Preferences):
- `https://dl.espressif.com/dl/package_esp32_index.json`
- `https://github.com/earlephilhower/arduino-pico/releases/download/global/package_rp2040_index.json`

## Key pin assignments

| Signal             | Chip  | GPIO |
```

</details>
