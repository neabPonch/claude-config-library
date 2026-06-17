---
name: nikhilmethi__zephyr-rtos
source: https://github.com/nikhilmethi/zephyr-rtos/blob/d74d925495949f3dafdec50b4fbfabff53e28c2a/CLAUDE.md
repo: nikhilmethi/zephyr-rtos
kind: claude-md
stars: 0
last_pushed: 2026-04-27T17:03:53Z
license: unknown
score: 8
domains: [embedded-systems, firmware]
tags: [zephyr, rtos, nrf52, west]
curated: 2026-06-16
curated_by: config-scout
---

# nikhilmethi/zephyr-rtos — claude-md

**Why it's worth keeping:** The 'Key Conventions' and 'Architecture' sections are excellent; they explain how to enable features via Kconfig/Devicetree, which is crucial context for AI assisting with hardware-dependent code.

**Summary:** Provides specific build and test instructions for an embedded Zephyr RTOS project using the west toolchain and Python pytest.

**Source credibility:** Academic lab repository from a Duke University course (BME 554).

**Recency:** Current; follows modern Zephyr/West and Python testing workflows.

**Source:** [nikhilmethi/zephyr-rtos/CLAUDE.md](https://github.com/nikhilmethi/zephyr-rtos/blob/d74d925495949f3dafdec50b4fbfabff53e28c2a/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Duke BME 554 (Embedded Medical Devices) lab repository for ECG, temperature sensing, and BLE on the **nRF52833 Development Kit**. Built on Zephyr RTOS using the nRF Connect SDK. Students progressively enable features (GPIO, timers, ADC, PWM, I2C, BLE) through lab exercises.

## Build Commands

### Zephyr Application (requires nRF Connect SDK / west)

```bash
# Initialize west workspace (first time only, run from repo root)
west init -l application
west update

# Build the application
west build application --pristine -b nrf52833dk/nrf52833 --no-sysbuild

# Flash to board
west flash
```

The CMake preset in `application/CMakePresets.json` configures the board target and overlay automatically for IDE builds (nRF Connect for VS Code extension).

### Python Tests

```bash
# Install dependencies
conda env create -f environment.yml   # or: pip install -r requirements.txt

# Run all tests
pytest -v testing/

# Run a single test
pytest -v testing/test_bme554.py::test_read_hex_data
```

## Architecture

### `application/` — Zephyr Embedded Firmware

- **`
```

</details>
