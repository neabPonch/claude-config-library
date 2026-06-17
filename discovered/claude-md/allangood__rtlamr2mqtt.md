---
name: allangood__rtlamr2mqtt
source: https://github.com/allangood/rtlamr2mqtt/blob/3869cdf84fd3d4ac5b6a07b62eee74905f3dc6c3/CLAUDE.md
repo: allangood/rtlamr2mqtt
kind: claude-md
stars: 490
last_pushed: 2026-06-15T04:30:34Z
license: mit
score: 9
domains: [iot, python-backend, embedded-systems, docker]
tags: [asyncio, mqtt, process-management, hardware-integration]
curated: 2026-06-16
curated_by: config-scout
---

# allangood/rtlamr2mqtt — claude-md

**Why it's worth keeping:** It explains the 'mental model' of the system (TaskGroups, Queues, and Signal handling) rather than just listing files. The specific details on subprocess buffering (stdbuf) and lifecycle logic are invaluable for preventing regressions.

**Summary:** A highly technical guide for an async Python service that bridges hardware data to MQTT. It provides deep context on process management, task synchronization, and dual-mode runtime detection.

**Source credibility:** Strong; 490 stars and very recent maintenance suggest a stable, well-used tool.

**Recency:** Extremely current, utilizing modern Python patterns like asyncio.TaskGroup.

**Source:** [allangood/rtlamr2mqtt/CLAUDE.md](https://github.com/allangood/rtlamr2mqtt/blob/3869cdf84fd3d4ac5b6a07b62eee74905f3dc6c3/CLAUDE.md) · 490★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**rtlamr2mqtt** bridges RTL-SDR radio receivers to MQTT, enabling Home Assistant to read utility meters (electric, gas, water). It runs either as a **Home Assistant add-on** or a **standalone Docker container**. The v2026 rewrite replaced blocking subprocess calls with a fully async architecture.

All application code lives under `rtlamr2mqtt-addon/` — this is both the Docker build context and the HA add-on root.

## Commands

All commands run from `rtlamr2mqtt-addon/`:

```bash
# Set up dev environment
python3 -m venv .venv
.venv/bin/pip install -r requirements-dev.txt

# Run all tests
.venv/bin/pytest

# Run a single test file
.venv/bin/pytest tests/test_process_manager.py -v

# Run a single test by name
.venv/bin/pytest tests/test_config.py -v -k "test_load_standalone"

# Lint
.venv/bin/pylint --rcfile=.pylint app/

# Build Docker image (standalone mode)
docker build -t rtlamr2mqtt .

# Integration test with mock RTL-SDR hardware
docker compose up --build
# In another terminal, subscribe to verify output:
docker exec rtlamr2mqtt-addon-mosquitt
```

</details>
