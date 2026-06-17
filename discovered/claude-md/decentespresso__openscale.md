---
name: decentespresso__openscale
source: https://github.com/decentespresso/openscale/blob/9d4ac4c31b1027a9a6a5a484e15bf59e59386ce6/CLAUDE.md
repo: decentespresso/openscale
kind: claude-md
stars: 83
last_pushed: 2026-06-09T09:02:22Z
license: gpl-3.0
score: 10
domains: [embedded-systems, iot]
tags: [esp32, firmware, concurrency, hardware]
curated: 2026-06-16
curated_by: config-scout
---

# decentespresso/openscale — claude-md

**Why it's worth keeping:** It defines critical 'footguns' regarding task concurrency and radio coexistence using a resource safety table; it also explains an unusual unity-build file structure to prevent architectural errors.

**Summary:** Highly technical instructions for ESP32-S3 espresso scale firmware, covering build workflows and hardware-specific constraints.

**Source credibility:** Strong; high-quality project with very recent activity and specific hardware context.

**Recency:** Highly current, reflecting modern PlatformIO/ESP32 development patterns.

**Source:** [decentespresso/openscale/CLAUDE.md](https://github.com/decentespresso/openscale/blob/9d4ac4c31b1027a9a6a5a484e15bf59e59386ce6/CLAUDE.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Half Decent Scale firmware

Espresso-scale firmware for the HDS hardware: ESP32-S3 + load-cell amplifier (ADS1232 or HX711) + 128x64 OLED + BLE + WiFi. Built with PlatformIO + Arduino framework. The on-device web app at `/` talks to the firmware over a single `/snapshot` WebSocket.

## Quick reference

```sh
# All commands run from the repo root.
pio run -e esp32s3                                                # build
pio run -e esp32s3 -t upload --upload-port /dev/cu.wchusbserial110 # flash firmware
pio run -e esp32s3 -t uploadfs --upload-port /dev/cu.wchusbserial110 # flash LittleFS (web_apps/)
```

```sh
# Serial monitor — pio device monitor needs a PTY. From a non-tty harness use
# pyserial directly. Path is the PlatformIO-bundled python so pyserial is on
# its sys.path; system python3 typically isn't.
/opt/homebrew/Cellar/platformio/6.1.19_1/libexec/bin/python3 -u -c "
import serial, sys
s = serial.Serial('/dev/cu.wchusbserial110', 115200, timeout=1)
while True:
    line = s.readline()
    if line:
        sys.stdout.write(line.decode('utf-8', errors='replace'))
        sys.stdout.flush()
"
```

The scale advertises mDNS `hds.local` plus a DNS-SD service `_decen
```

</details>
