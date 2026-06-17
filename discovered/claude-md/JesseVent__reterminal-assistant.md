---
name: JesseVent__reterminal-assistant
source: https://github.com/JesseVent/reterminal-assistant/blob/7b345aca7c40a0709f7a794f42973083e8f912f4/CLAUDE.md
repo: JesseVent/reterminal-assistant
kind: claude-md
stars: 0
last_pushed: 2026-05-30T10:49:31Z
license: apache-2.0
score: 9
domains: [embedded, iot]
tags: [esp-idf, bsp, hardware-sdk]
curated: 2026-06-16
curated_by: config-scout
---

# JesseVent/reterminal-assistant — claude-md

**Why it's worth keeping:** It includes a visual dependency graph of the BSP, detailed I2C bus/pin mappings, and crucial runtime requirements like thread-safety (mutex) protocols for the UI framework.

**Summary:** This file provides comprehensive hardware and software context for an embedded ESP32-P4 project, covering component dependencies and specific build workflows.

**Source credibility:** Highly technical documentation from a niche hardware SDK repository.

**Recency:** Very recent; updated within the last month.

**Source:** [JesseVent/reterminal-assistant/CLAUDE.md](https://github.com/JesseVent/reterminal-assistant/blob/7b345aca7c40a0709f7a794f42973083e8f912f4/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

reTerminal D1001 SDK by Seeed Studio — an embedded firmware project for the reTerminal D1001 IoT device based on the **ESP32-P4** MCU. Built on **ESP-IDF v5.4.2** (compatible with v5.3+). The device features an 800×1280 MIPI DSI LCD (JD9365), capacitive touch (GSL3670), camera (SC2356), audio codecs (ES8311 DAC / ES7210 ADC), IMU (LSM6DS3), RTC (PCF8563), IO expander (PCA9535), battery management, Wi-Fi (via ESP-Hosted over SDIO to ESP32-C6 slave), LTE modem (USB), and LoRa (SPI).

## Build System

Uses ESP-IDF's `idf.py` build system (CMake-based). **Target is always `esp32p4`.**

```bash
# Set target (required once per project)
idf.py set-target esp32p4

# Build
idf.py build

# Flash and monitor (replace /dev/ttyACM0 with actual serial port)
idf.py --port /dev/ttyACM0 flash monitor

# Combined build + flash + monitor
idf.py --port /dev/ttyACM0 build flash monitor

# Erase flash
idf.py --port /dev/ttyACM0 erase-flash
```

Exit serial monitor with `Ctrl+]`.

## Repository Structure

- **`components/`** — Reusable ESP-IDF components (board support
```

</details>
