---
name: tuya__DuckyClaw
source: https://github.com/tuya/DuckyClaw/blob/3d03e8da77e70cb1647d1f33acfce3b33149e1c1/CLAUDE.md
repo: tuya/DuckyClaw
kind: claude-md
stars: 135
last_pushed: 2026-05-15T07:13:47Z
license: apache-2.0
score: 9
domains: [embedded-systems, ai-agents, iot]
tags: [C, hardware, edge-computing, tuya-sdk]
curated: 2026-06-15
curated_by: config-scout
---

# tuya/DuckyClaw — claude-md

**Why it's worth keeping:** The 'Key Patterns' section is exceptional for teaching an LLM project-specific idioms like memory management and error handling macros, while the build section includes practical automation hacks.

**Summary:** Provides comprehensive architectural mapping and specific low-level development instructions for an edge-computing AI agent.

**Source credibility:** A specialized repository with decent community interest (135 stars) focused on hardware/IoT integration.

**Recency:** Highly current; pushed within the last month.

**Source:** [tuya/DuckyClaw/CLAUDE.md](https://github.com/tuya/DuckyClaw/blob/3d03e8da77e70cb1647d1f33acfce3b33149e1c1/CLAUDE.md) · 135★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DuckyClaw is a hardware-oriented AI agent built on the TuyaOpen C SDK. It runs a Claw-style agent loop on edge devices (Tuya T5AI, ESP32, Raspberry Pi, Linux) that communicates with users via IM channels (Telegram, Discord, Feishu) and executes MCP-style tools on the device.

## Build Commands

DuckyClaw builds as a TuyaOpen application. From the repo root:

```bash
# Initialize TuyaOpen environment (creates .venv, exports OPEN_SDK_ROOT)
cd TuyaOpen && . ./export.sh && cd ..

# Select board config (copies to app_default.config)
# Available configs are in config/ directory
cp config/RaspberryPi.config app_default.config           # Raspberry Pi
cp config/TUYA_T5AI_BOARD_LCD_3.5_CAMERA.config app_default.config  # Tuya T5AI
cp config/ESP32S3_BREAD_COMPACT_WIFI.config app_default.config      # ESP32-S3

# Build (from TuyaOpen directory, pointing to DuckyClaw as the app)
cd TuyaOpen
python3 tos.py build

# Output goes to dist/ directory
# For LINUX target: produces native ELF binary
```

To skip interactive platform prompts during builds:
```bash
mkd
```

</details>
