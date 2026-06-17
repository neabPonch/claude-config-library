---
name: QuickRecon__DiveCANHead
source: https://github.com/QuickRecon/DiveCANHead/blob/75b29323fbccd45f22e00cf6a00f512da2bfcd2c/CLAUDE.md
repo: QuickRecon/DiveCANHead
kind: claude-md
stars: 13
last_pushed: 2026-05-14T11:47:50Z
license: mit
score: 9
domains: [embedded, firmware]
tags: [stm32, freertos, safety-critical, mcp]
curated: 2026-06-15
curated_by: config-scout
---

# QuickRecon/DiveCANHead — claude-md

**Why it's worth keeping:** The 'NASA Rules of 10' section enforces strict safety patterns essential for embedded systems, while the task architecture provides vital understanding of system concurrency. The inclusion of specialized MCP tool commands makes it highly effective for agentic workflows.

**Summary:** This file provides deep architectural context, build/test workflows, and safety-critical coding standards for an STM32 FreeRTOS project. It also includes specific instructions for using MCP tools to query static analysis results.

**Source credibility:** Highly credible; specific to a niche, technical hardware project with clear engineering rigor.

**Recency:** Very recent; incorporates modern instructions for interacting with MCP-based static analysis tools.

**Source:** [QuickRecon/DiveCANHead/CLAUDE.md](https://github.com/QuickRecon/DiveCANHead/blob/75b29323fbccd45f22e00cf6a00f512da2bfcd2c/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is firmware for a DiveCAN-compatible PPO2 monitoring and control head for closed-circuit rebreathers (CCRs). The system interfaces with oxygen sensors (both analog and digital), manages solenoid control via PID loop, and communicates with Shearwater dive computers over the DiveCAN bus.

The hardware is based on an STM32L4 microcontroller running FreeRTOS with dual-rail power (VCC for critical systems, VBUS for peripherals), external ADCs for analog oxygen sensors, UARTs for digital sensors, SD card logging, and CAN bus communication.

## Build Commands

### Firmware (STM32)

```bash
# Build firmware
cd STM32
make

# Build output: STM32/build/STM32.hex and STM32/build/STM32.bin
```

### Unit Tests (C/C++)

```bash
# First time setup - build cpputest
cd STM32/Tests/cpputest
autoreconf -i
./configure
make

# Build and run unit tests
cd STM32/Tests
make
```

### Hardware Tests (Python/pytest)

```bash
# Install dependencies
pip install -r requirements.txt

# Run hardware integration tests
cd "HW Testing/Tests"
pytest

# Run specific test file
py
```

</details>
