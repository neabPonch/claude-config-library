---
name: smittix__intercept
source: https://github.com/smittix/intercept/blob/b68a53eb53a699817b501b07d1d12491154dce82/CLAUDE.md
repo: smittix/intercept
kind: claude-md
stars: 1892
last_pushed: 2026-05-21T21:07:46Z
license: apache-2.0
score: 9
domains: [iot, signal-intelligence, systems-programming]
tags: [hardware-integration, real-time-streaming, subprocess-management]
curated: 2026-06-15
curated_by: config-scout
---

# smittix/intercept — claude-md

**Why it's worth keeping:** It includes explicit procedural checklists for feature integration (Frontend Mode Integration) and detailed mapping of how external tools interact with the core system. This prevents an agent from breaking delicate process lifecycles or SSE patterns.

**Summary:** A high-density technical manual for a complex SIGINT platform that details hardware abstraction, subprocess management, and real-time streaming architectures.

**Source credibility:** Highly credible; the 1.8k+ stars indicate a significant, well-maintained open-source project.

**Recency:** Current; reflects modern development tooling like ruff and specific docker-compose profiles.

**Source:** [smittix/intercept/CLAUDE.md](https://github.com/smittix/intercept/blob/b68a53eb53a699817b501b07d1d12491154dce82/CLAUDE.md) · 1892★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

INTERCEPT is a web-based Signal Intelligence (SIGINT) platform providing a unified Flask interface for software-defined radio (SDR) tools. It supports pager decoding, 433MHz sensors, ADS-B aircraft tracking, ACARS messaging, WiFi/Bluetooth scanning, satellite tracking, ISS SSTV decoding, AIS vessel tracking, weather satellite imagery (NOAA APT & Meteor LRPT), and Meshtastic mesh networking.

## Common Commands

### Docker (Primary)
```bash
# Build and run (basic profile)
docker compose --profile basic up -d

# Build and run with ADS-B history (Postgres)
docker compose --profile history up -d

# Rebuild after code changes
docker compose --profile basic up -d --build

# Multi-arch build (amd64 + arm64 for RPi)
./build-multiarch.sh
```

### Local Setup (Alternative)
```bash
# First-time setup (interactive wizard with install profiles)
./setup.sh

# Or headless full install
./setup.sh --non-interactive

# Or install specific profiles
./setup.sh --profile=core,weather

# Run with production server (gunicorn + gevent, handles concurrent SSE/WebSocket)
```

</details>
