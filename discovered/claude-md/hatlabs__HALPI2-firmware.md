---
name: hatlabs__HALPI2-firmware
source: https://github.com/hatlabs/HALPI2-firmware/blob/be8d172875a238d39450a01c4f45c225ff6e8c1e/CLAUDE.md
repo: hatlabs/HALPI2-firmware
kind: claude-md
stars: 1
last_pushed: 2026-04-23T19:04:58Z
license: mit
score: 9
domains: [embedded, rust]
tags: [firmware, rust-embassy, cli-wrapper]
curated: 2026-06-16
curated_by: config-scout
---

# hatlabs/HALPI2-firmware — claude-md

**Why it's worth keeping:** The pattern of wrapping complex toolchains into a unified `./run` script is perfect for AI agents; it also provides critical domain-specific state machine logic and strict 'Never' instructions to prevent manual error.

**Summary:** Provides a highly structured technical overview of an embedded Rust project and defines a single CLI entry point for all development tasks.

**Source credibility:** Low star count, but the technical depth suggests a high-quality professional embedded project.

**Recency:** Very recent (2 months ago), highly relevant for modern agentic workflows.

**Source:** [hatlabs/HALPI2-firmware/CLAUDE.md](https://github.com/hatlabs/HALPI2-firmware/blob/be8d172875a238d39450a01c4f45c225ff6e8c1e/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

HALPI2 is a Raspberry Pi Compute Module 5 based boat computer with an RP2040 microcontroller handling power management and peripheral control. The firmware is written in Rust using the Embassy async framework.

## Development Commands

Use the `./run` script for all development tasks. Commands are organized by functional area:

### Core Development
- `./run build [--release]` - Build firmware (debug by default)
- `./run build:bootloader [--release]` - Build bootloader
- `./run clean` - Clean all build artifacts
- `./run check` - Run cargo check and clippy

### Hardware Interaction
- `./run flash [firmware|bootloader|all]` - Flash to device (default: firmware)
- `./run monitor` - Attach debugger/monitor
- `./run flash:monitor` - Flash then monitor (common workflow)

### Release/Artifacts
- `./run release:build` - Build all release artifacts (elf, bin, uf2)
- `./run release:artifacts` - Convert existing ELF to bin/uf2 formats
- `./run release:version` - Get current firmware version

### Package Management
- `./run package:deb` - Build Debian packag
```

</details>
