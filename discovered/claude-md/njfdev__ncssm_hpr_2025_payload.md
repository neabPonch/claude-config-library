---
name: njfdev__ncssm_hpr_2025_payload
source: https://github.com/njfdev/ncssm_hpr_2025_payload/blob/64ecd1bf9b7d041cb11aa87e014513ff4de1978f/CLAUDE.md
repo: njfdev/ncssm_hpr_2025_payload
kind: claude-md
stars: 2
last_pushed: 2026-04-20T23:39:42Z
license: unknown
score: 9
domains: [embedded, rust]
tags: [skill-management, knowledge-persistence, automation]
curated: 2026-06-15
curated_by: config-scout
---

# njfdev/ncssm_hpr_2025_payload — claude-md

**Why it's worth keeping:** It introduces a sophisticated 'Skill Maintenance' protocol where the AI is required to update structured documentation after every session, creating persistent institutional memory. It also includes practical automation patterns like using helper scripts over direct commands and audible user alerts.

**Summary:** A comprehensive guide for a multi-component Rust embedded project that establishes a high-level framework for agent learning and hardware interaction.

**Source credibility:** A specialized student rocket payload project with specific hardware-software integration requirements.

**Recency:** Current; uses modern Claude Code strategies such as context compaction and structured skill files.

**Source:** [njfdev/ncssm_hpr_2025_payload/CLAUDE.md](https://github.com/njfdev/ncssm_hpr_2025_payload/blob/64ecd1bf9b7d041cb11aa87e014513ff4de1978f/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

NCSSM Rocketry 2025 Payload - A multi-component Rust embedded systems project for a high-altitude rocket. The system consists of three packages that work together: a flight computer for high-level processing and camera capture, a Pico-based data logger for sensor telemetry, and a ground station for mission control.

## Build Commands

### Flight Computer (Linux host, camera/video processing)
```bash
cd flight_computer
cargo build --release
cargo run --release
```
**Prerequisites**: Requires `ffmpeg-rk` (not regular ffmpeg) for hardware encoding and PipeWire audio system.

### Pico Logger (RP2040 embedded firmware)
```bash
cd pico_logger
cargo build --release
cargo run --release  # Uses picotool to flash (device must be in BOOTSEL mode)
```
**Prerequisites**: Requires `picotool` installed for flashing. Target is `thumbv6m-none-eabi` (ARMv6-M Cortex-M0+).

### Ground Station
```bash
cd ground_station
cargo build --release
cargo run --release
```

## Architecture

### Three-Package Structure
- **flight_computer/**: High-level processing unit running
```

</details>
