---
name: rob-brown__amo_system
source: https://github.com/rob-brown/amo_system/blob/9bb5db336bf7b7c790ce63edd14018f5656ca65c/CLAUDE.md
repo: rob-brown/amo_system
kind: claude-md
stars: 2
last_pushed: 2026-02-13T19:22:44Z
license: mit
score: 9
domains: [embedded, elixir, automation, computer-vision]
tags: [monorepo, hardware, firmware, elixir]
curated: 2026-06-15
curated_by: config-scout
---

# rob-brown/amo_system — claude-md

**Why it's worth keeping:** Includes a dependency graph to map component relationships; features high-value 'Gotchas' regarding environment constraints (e.g., avoiding interactive `iex` in automated contexts).

**Summary:** Comprehensive guidance for a hardware-interfacing monorepo involving Elixir applications, C firmware, and computer vision. It provides essential architectural context for navigating multi-component automation systems.

**Source credibility:** The content reflects deep technical expertise and structural clarity despite the low star count.

**Recency:** Highly current, referencing modern hardware like the Raspberry Pi Pico 2 W.

**Source:** [rob-brown/amo_system/CLAUDE.md](https://github.com/rob-brown/amo_system/blob/9bb5db336bf7b7c790ce63edd14018f5656ca65c/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the **Amiibo Modular Open System (AMO System)** - a comprehensive toolkit for working with and automating amiibo on Nintendo Switch. The system includes:

- Bluetooth controller emulation (Pro Controller, Joy-Con)
- Computer vision for automated gameplay
- Amiibo file reading/writing and encryption/decryption
- Tournament automation for Super Smash Bros. Ultimate
- Web interface for amiibo management
- Embedded firmware for Raspberry Pi Pico 2 W

## Repository Structure

This is a **monorepo** containing multiple independent Elixir applications with local path dependencies, plus embedded C firmware:

- **apps/** - Independent Elixir applications (not an Umbrella project)
- **firmware/** - Embedded C firmware projects
- **notebooks/** - Livebook notebooks for interactive workflows
- **docs/** - Documentation

## Key Applications

### Core Libraries

- **amiibo_serialization** - Read/write/encrypt/decrypt amiibo files (based on PyAmiibo)
- **ssbu** - Extract SSBU-specific information from amiibo (character data, stats)
- **vision** - Comput
```

</details>
