---
name: adawolfs__ESP-igivice
source: https://github.com/adawolfs/ESP-igivice/blob/70d8b0325b21a1ac4311df6563bb452ff9dceb07/CLAUDE.md
repo: adawolfs/ESP-igivice
kind: claude-md
stars: 0
last_pushed: 2026-04-27T01:59:44Z
license: unknown
score: 9
domains: [embedded, iot, firmware]
tags: [esp32, platformio, hardware-interfacing, asset-pipeline]
curated: 2026-06-16
curated_by: config-scout
---

# adawolfs/ESP-igivice — claude-md

**Why it's worth keeping:** The 'Hardware Target' and 'Pin Map' tables provide essential physical context; the 'Common Pitfalls' section includes vital hardware tuning advice (SPI frequency/color inversion) that prevents logic errors.

**Summary:** A high-quality embedded systems guide providing critical hardware context, pin maps, and asset-generation workflows. It bridges the gap between source code and physical hardware constraints.

**Source credibility:** Low social proof due to 0 stars, but the technical density suggests a high-quality personal project.

**Recency:** Current; aligns with modern PlatformIO and ESP32 development workflows.

**Source:** [adawolfs/ESP-igivice/CLAUDE.md](https://github.com/adawolfs/ESP-igivice/blob/70d8b0325b21a1ac4311df6563bb452ff9dceb07/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Build & Flash Commands

```bash
# Build firmware
pio run

# Build and upload to connected ESP32-C3
pio run --target upload

# Open serial monitor
pio device monitor

# Clean build artifacts
pio run --target clean
```

There are no automated tests. This is embedded firmware targeting physical
hardware.

## Hardware Target

| Item | Value |
| --- | --- |
| MCU | ESP32-C3 |
| Board | `esp32-c3-devkitm-1` |
| Display | GC9A01 round 240x240 TFT via SPI2 |
| Touch | CST816D capacitive touch over I2C |
| Framework | Arduino via PlatformIO |

## Pin Map

| Signal | GPIO |
| --- | --- |
| SPI MOSI | 7 |
| SPI SCLK | 6 |
| TFT CS | 10 |
| TFT DC | 2 |
| Backlight | 3 |
| I2C SDA | 4 |
| I2C SCL | 5 |
| Touch INT | 0 |
| Touch RST | 1 |

## Architecture

The current firmware is a direct LovyanGFX renderer. It does not use LVGL at
runtime. `src/main.cpp` initializes the GC9A01 panel, initializes the CST816D
touch controller, mounts SPIFFS, and plays a GIF animation from
`data/gif/current.gif`.

The bitmap source is `Untitled-2.png`. It is converted ahead of time into
`include
```

</details>
