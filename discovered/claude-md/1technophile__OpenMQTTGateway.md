---
name: 1technophile__OpenMQTTGateway
source: https://github.com/1technophile/OpenMQTTGateway/blob/0b6780678f601041b7f4d63c8e087665c335d8ff/CLAUDE.md
repo: 1technophile/OpenMQTTGateway
kind: claude-md
stars: 4024
last_pushed: 2026-06-14T22:20:28Z
license: gpl-3.0
score: 9
domains: [embedded, iot]
tags: [platformio, esp32, mqtt, firmware]
curated: 2026-06-15
curated_by: config-scout
---

# 1technophile/OpenMQTTGateway — claude-md

**Why it's worth keeping:** The 'Common Patterns' section provides precise, actionable templates for adding new modules and explains the specific configuration override pattern.

**Summary:** Provides high-level architecture, complex build system mechanics, and explicit recipes for extending the firmware with new modules.

**Source credibility:** High; a widely used project with 4k+ stars and very recent maintenance.

**Recency:** Current; includes modern build-system details suitable for today's AI assistance.

**Source:** [1technophile/OpenMQTTGateway/CLAUDE.md](https://github.com/1technophile/OpenMQTTGateway/blob/0b6780678f601041b7f4d63c8e087665c335d8ff/CLAUDE.md) · 4024★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenMQTTGateway - Claude Code Context

This document provides essential context about the OpenMQTTGateway project for AI assistants working on the codebase.

## Project Overview

OpenMQTTGateway is a unified firmware that bridges various wireless technologies (RF 433MHz, IR, BLE, LoRa, etc.) to MQTT protocol, enabling home automation integration with platforms like Home Assistant, OpenHAB, and Node-RED.

**Key Features:**
- Multi-protocol gateway (BLE, RF 433MHz, IR, LoRa, RTL_433, Pilight, etc.)
- ESP8266/ESP32 and Arduino support
- MQTT-based communication
- Web UI for configuration
- Home Assistant MQTT Discovery support
- Over 100 supported BLE sensors via Theengs Decoder

**Main Branch:** `development` (not master/main)

## Architecture

### Modular Design

The firmware uses a modular architecture where each protocol/sensor/actuator is implemented as a separate "gateway" or "sensor" module:

- **Gateways**: Receive and transmit signals (e.g., `gatewayBT.cpp`, `gatewayRF.cpp`, `gatewayIR.cpp`)
- **Sensors**: Read physical sensor data (e.g., `sensorBME280.cpp`, `sensorDHT.cpp`)
- **Actuators**: Control outputs (e.g., `actuatorONOFF.cpp`, `actuatorPWM.cpp`)

Each module has:
-
```

</details>
