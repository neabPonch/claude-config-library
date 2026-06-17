---
name: sanghviharshit__wandering-hour-clock
source: https://github.com/sanghviharshit/wandering-hour-clock/blob/41bbce27ef1ba710ac22bb584586fd09dff8a46b/CLAUDE.md
repo: sanghviharshit/wandering-hour-clock
kind: claude-md
stars: 10
last_pushed: 2026-04-06T02:21:36Z
license: gpl-3.0
score: 9
domains: [embedded-systems, iot]
tags: [esp32, arduino, hardware-interface]
curated: 2026-06-16
curated_by: config-scout
---

# sanghviharshit/wandering-hour-clock — claude-md

**Why it's worth keeping:** Explicitly documents low-level hardware details (pins, motor step math) and network failure modes that prevent AI from suggesting blocking or invalid code.

**Summary:** Highly effective documentation for hardware-software interaction, covering pinouts, library dependencies, and specific logic math.

**Source credibility:** Decent niche project with 10 stars and recent updates.

**Recency:** Current and highly relevant for modern ESP32/Arduino development workflows.

**Source:** [sanghviharshit/wandering-hour-clock/CLAUDE.md](https://github.com/sanghviharshit/wandering-hour-clock/blob/41bbce27ef1ba710ac22bb584586fd09dff8a46b/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Wandering Hour Clock

## Project Overview

This is an Arduino/C++ project for an ESP32-based WiFi-connected wandering hour clock. It drives a 28BYJ-48 stepper motor to display time using a wandering hour mechanism, syncs time via NTP, and exposes a web UI for manual adjustments and preferences.

**Single source file:** `wandering-hour-clock.ino` (Arduino sketch, ~580 lines)

---

## Repository Structure

```
wandering-hour-clock/
├── wandering-hour-clock.ino   # Main Arduino sketch (all logic lives here)
├── secrets.h                  # WiFi credentials (gitignored, must be created locally)
├── README.md                  # User-facing documentation and hardware instructions
├── LICENSE                    # GPLv3
└── images/                    # Photos, wiring diagrams, and demo GIFs
```

---

## Hardware Platform

- **MCU:** ESP32 (or ESP8266) with WiFi
- **Motor:** 28BYJ-48 unipolar stepper motor (2048 steps/revolution)
- **Driver:** ULN2003
- **Motor pins:** IN1=19, IN2=18, IN3=5, IN4=17
- **Built-in LED:** pin 13
- **Power:** 5V, 2A+

---

## Arduino Libraries Required

Install these in Arduino IDE before compiling:

| Library | Purpose | Source |
|---|---|---|
| `
```

</details>
