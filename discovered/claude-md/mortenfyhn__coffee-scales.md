---
name: mortenfyhn__coffee-scales
source: https://github.com/mortenfyhn/coffee-scales/blob/5ec7c391cdbb1422223cdcbac54af3a6f5168fa0/CLAUDE.md
repo: mortenfyhn/coffee-scales
kind: claude-md
stars: 24
last_pushed: 2026-03-23T06:39:05Z
license: gpl-3.0
score: 9
domains: [embedded-systems, firmware]
tags: [state-machine, signal-processing, platformio, hardware]
curated: 2026-06-15
curated_by: config-scout
---

# mortenfyhn/coffee-scales — claude-md

**Why it's worth keeping:** Explains the 'how' of algorithms (filtering/state transitions) rather than just file structure; includes specific instructions for validating code changes against external data analysis tools like Jupyter/Octave.

**Summary:** Provides deep context for an embedded firmware project, detailing a complex signal processing pipeline and state machine. It connects low-level hardware interaction with high-level mathematical validation workflows.

**Source credibility:** Niche project with highly specialized, high-quality technical documentation.

**Recency:** Very recent; updated within the last few months.

**Source:** [mortenfyhn/coffee-scales/CLAUDE.md](https://github.com/mortenfyhn/coffee-scales/blob/5ec7c391cdbb1422223cdcbac54af3a6f5168fa0/CLAUDE.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an embedded firmware project for custom coffee scales designed for drip coffee brewing. The scales feature:
- 0.1 gram precision with quick response
- Auto-starting brew timer
- Auto-off after 5 minutes
- State machine-based control (taring, ready, brewing, dim, sleep)

## Build System

The project uses **PlatformIO** for firmware builds and **Just** as a command runner. All commands should be run from the repository root.

### Essential Commands

```sh
# Build firmware (release configuration)
just build

# Build and upload to connected board
just upload

# Run unit tests
just test

# Build and upload debug firmware, then monitor serial output
just debug

# Upload logging firmware and capture/process logs
just log
```

### Build Environments

PlatformIO defines multiple environments in `firmware/platformio.ini`:
- `release` (default): Production firmware
- `logging`: Enables CSV logging via serial for debugging
- `debug`: Debug build with serial output
- `test`: Native unit tests (runs on host, not on device)

Build specific environment:
```

</details>
