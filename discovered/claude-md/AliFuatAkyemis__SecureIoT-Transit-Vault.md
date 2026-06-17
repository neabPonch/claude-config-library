---
name: AliFuatAkyemis__SecureIoT-Transit-Vault
source: https://github.com/AliFuatAkyemis/SecureIoT-Transit-Vault/blob/47b66869169b92921b1995b33844023de8a52c38/CLAUDE.md
repo: AliFuatAkyemis/SecureIoT-Transit-Vault
kind: claude-md
stars: 0
last_pushed: 2026-05-08T10:49:28Z
license: mit
score: 8
domains: [embedded-systems, iot]
tags: [esp32, arduino, hardware-integration]
curated: 2026-06-15
curated_by: config-scout
---

# AliFuatAkyemis/SecureIoT-Transit-Vault — claude-md

**Why it's worth keeping:** It includes a practical workflow for capturing RFID UIDs via Serial Monitor and explicitly defines I2C pin assignments and sensor thresholds to prevent logic errors during code generation.

**Summary:** Provides highly specific hardware mappings, library version requirements, and crucial warnings regarding auto-generated cloud files.

**Source credibility:** Low social proof (0 stars) from a single developer.

**Recency:** Current; reflects modern ESP32/Arduino development workflows.

**Source:** [AliFuatAkyemis/SecureIoT-Transit-Vault/CLAUDE.md](https://github.com/AliFuatAkyemis/SecureIoT-Transit-Vault/blob/47b66869169b92921b1995b33844023de8a52c38/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ESP32-based IoT vault with RFID access control, tamper detection, remote cloud control, and OLED status display. Deployed via Arduino IDE or Arduino Cloud editor.

**Target board:** ESP32 DOIT DevKit V1 (`esp32:esp32:esp32doit-devkit-v1`)

## Build & Upload

Arduino IDE or Arduino Cloud — no CLI build system. Use Arduino IDE 2.x:

1. Open `SecureIoT_Transit_Vault/SecureIoT_Transit_Vault.ino`
2. Select board: **DOIT ESP32 DEVKIT V1**
3. Install required libraries (see below)
4. Fill `arduino_secrets.h` with credentials
5. Upload via USB

To read RFID card UIDs: open Serial Monitor at **115200 baud**, tap a card, copy UID from `[RFID] Card UID:` line, add to `AUTHORIZED_UIDS[]` in `.ino`.

## Required Libraries

| Library | Version |
|---|---|
| Adafruit SSD1306 | 2.5.10 |
| Adafruit GFX Library | 1.11.9 |
| MFRC522 | 1.4.10 |
| MPU6050_tockn | 1.0.2 |
| ESP32Servo | 0.13.0 |
| ArduinoIoTCloud | (via Arduino Cloud) |
| Arduino_ConnectionHandler | (via Arduino Cloud) |

## File Structure

- `SecureIoT_Transit_Vault.ino` — main logic: setup/loop, har
```

</details>
