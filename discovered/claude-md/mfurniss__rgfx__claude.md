---
name: mfurniss__rgfx__claude
source: https://github.com/mfurniss/rgfx/blob/0798d20b0f521cd3d3a3b551bd48e3d804c56967/esp32/src/network/CLAUDE.md
repo: mfurniss/rgfx
kind: claude-md
stars: 5
last_pushed: 2026-05-28T04:35:12Z
license: mpl-2.0
score: 9
domains: [embedded-systems, iot, firmware]
tags: [esp32, multicore, mqtt, concurrency]
curated: 2026-06-15
curated_by: config-scout
---

# mfurniss/rgfx — claude-md

**Why it's worth keeping:** It provides explicit 'CRITICAL' warnings about thread safety and cross-core race conditions, which prevents the AI from introducing subtle concurrency bugs in embedded environments.

**Summary:** A high-density technical specification for an ESP32 network module that details task separation across dual cores and protocol specifics.

**Source credibility:** High; well-maintained 5-star repository focused on retro hardware effects.

**Recency:** Very recent (last pushed 1 month ago).

**Source:** [mfurniss/rgfx/esp32/src/network/CLAUDE.md](https://github.com/mfurniss/rgfx/blob/0798d20b0f521cd3d3a3b551bd48e3d804c56967/esp32/src/network/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Network Module

> **Keep this file updated!** After making changes in this folder, update this CLAUDE.md to reflect the current state.

This folder contains all network communication code for the ESP32 driver firmware, including MQTT messaging, UDP effects transport, OTA updates, and network service initialization.

## Architecture

The network module runs primarily on **Core 0** (the "protocol core") via `networkTask()`, keeping network operations separate from the LED rendering on Core 1. This dual-core architecture ensures smooth LED animations even during network activity.

### Communication Protocols

| Protocol | Purpose | QoS |
|----------|---------|-----|
| MQTT | Configuration, commands, telemetry, status | QoS 2 (exactly-once) |
| UDP | Real-time effect messages from Hub | Best-effort (low latency) |
| mDNS | Device discovery and OTA advertising | - |
| UDP Broadcast | MQTT broker discovery (SSDP-style) | - |

## Files

| File | Description |
|------|-------------|
| `mqtt.h/cpp` | MQTT client setup, connection lifecycle, topic management |
| `mqtt_callback.cpp` | MQTT message routing and deferred operation processing |
| `mqtt_discovery.cpp` | Broker discovery with fal
```

</details>
