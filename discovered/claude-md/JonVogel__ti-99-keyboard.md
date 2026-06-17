---
name: JonVogel__ti-99-keyboard
source: https://github.com/JonVogel/ti-99-keyboard/blob/886bbd1d8e59514eacb21edb1e1b8af44e7528fe/CLAUDE.md
repo: JonVogel/ti-99-keyboard
kind: claude-md
stars: 0
last_pushed: 2026-05-12T01:55:23Z
license: mit
score: 9.5
domains: [embedded, firmware]
tags: [esp32, ble, hardware-interface]
curated: 2026-06-15
curated_by: config-scout
---

# JonVogel/ti-99-keyboard — claude-md

**Why it's worth keeping:** It uses critical 'negative constraints' to prevent hardware destruction (e.g., the TXS0108E warning) and provides deep technical reasoning for architectural choices like BLE reconnection strategies.

**Summary:** A high-density technical guide covering hardware pitfalls, electrical constraints, and low-level firmware logic for an ESP32 project.

**Source credibility:** Highly credible; contains extremely specific electrical validation data and component-level troubleshooting history.

**Recency:** Very current; includes 2026 hardware validation dates.

**Source:** [JonVogel/ti-99-keyboard/CLAUDE.md](https://github.com/JonVogel/ti-99-keyboard/blob/886bbd1d8e59514eacb21edb1e1b8af44e7528fe/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TI-99/4A Keyboard Adapter

USB/BLE keyboard adapter for the TI-99/4A. ESP32-S3 module translates modern keyboard HID reports into the TI's 6x8 keyboard matrix via discrete BSS138 level shifters. Installed inside the TI with the original keyboard removed; powered from the TI's 12V rail through a buck converter.

Sketch: `ti-99-keyboard.ino` (Arduino-ESP32 3.3.7).
PCB: `pcb/ti99-kb-adapter.kicad_pro` (KiCad 10), regeneratable via `pcb/generate_kicad.py`.

## Hardware

- **MCU:** Hosyond ESP32-S3 N16R8 dev board (USB-C, ESP32-S3-WROOM-1, 16MB flash, 8MB PSRAM). Sold as "Hosyond 3Pack ESP32-S3 Development Board N16R8 MCU with Dual-Mode Wi-Fi Bluetooth Type-C, Compatible with Arduino IoT ESP32-S3-WROOM-1". The older mini-USB ESP32-S3-DevKitC-1 boards are **obsoleted for this project** — at least one unit browns out repeatedly during NimBLE init (3V3 LDO can't keep up with the BLE TX inrush). Confirmed working Hosyond unit MAC e0:72:a1:d4:fb:20.
- **Level shifters:** BSS138 discrete MOSFET shifters, BOB-12009 topology (SparkFun). 14 channels total, 10kΩ pull-ups to 3V3 (LV) and 5V (HV).
- **Power:** standalone 12V→5V buck converter from TI's 12V rail; PSU daisy-chains via J13 solder pa
```

</details>
