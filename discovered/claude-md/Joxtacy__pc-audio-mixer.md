---
name: Joxtacy__pc-audio-mixer
source: https://github.com/Joxtacy/pc-audio-mixer/blob/4584af9db23704ae2a97345fd46a4cb73af513ba/CLAUDE.md
repo: Joxtacy/pc-audio-mixer
kind: claude-md
stars: 0
last_pushed: 2026-03-21T19:06:58Z
license: apache-2.0
score: 8
domains: [embedded, rust, hardware]
tags: [rp2040, embedded-rust, adc, usb-serial]
curated: 2026-06-16
curated_by: config-scout
---

# Joxtacy/pc-audio-mixer — claude-md

**Why it's worth keeping:** It documents critical external context like GPIO pin assignments and baud rates that aren't visible in the logic alone. It also includes a host-side Python test command to facilitate end-to-end verification.

**Summary:** Provides essential hardware-to-software mappings, build instructions for embedded Rust, and serial communication protocols.

**Source credibility:** Small personal project with low social proof (0 stars).

**Recency:** Current; uses modern tools like probe-rs and uv.

**Source:** [Joxtacy/pc-audio-mixer/CLAUDE.md](https://github.com/Joxtacy/pc-audio-mixer/blob/4584af9db23704ae2a97345fd46a4cb73af513ba/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a PC Audio Mixer project using a Raspberry Pi Pico (RP2040) microcontroller. The firmware reads analog values from 3 slide potentiometers and sends the values to a PC via USB CDC (serial communication) in JSON format.

## Build and Development Commands

### Rust/Embedded Development

```bash
# Build the embedded firmware
cargo build --release

# Flash and run on the Pico with debugging output
cargo run

# Build without flashing
cargo build

# Alternative flashing with cargo-embed (if probe-rs is not available)
cargo embed
```

### Python Test Script

```bash
# Run the test script to monitor potentiometer values (using uv)
uv run test_pico_connection.py

# Or with pip
pip install pyserial
python test_pico_connection.py
```

## Architecture

### Hardware Configuration
- **Microcontroller**: Raspberry Pi Pico (RP2040)
- **ADC Inputs**:
  - Pot 1: GPIO26 (ADC0)
  - Pot 2: GPIO27 (ADC1)
  - Pot 3: GPIO28 (ADC2)
- **Communication**: USB CDC Serial at 115200 baud
- **Update Rate**: 20Hz (50ms delay between readings)

### Code Structure

**Main F
```

</details>
