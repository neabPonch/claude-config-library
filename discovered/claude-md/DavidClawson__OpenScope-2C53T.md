---
name: DavidClawson__OpenScope-2C53T
source: https://github.com/DavidClawson/OpenScope-2C53T/blob/6f45061fa22cb6a7f526fe7b9f4f1f3f14f4222a/CLAUDE.md
repo: DavidClawson/OpenScope-2C53T
kind: claude-md
stars: 57
last_pushed: 2026-06-14T14:09:07Z
license: gpl-3.0
score: 9
domains: [embedded-systems, firmware, reverse-engineering]
tags: [arm-cortex, freertos, hardware-interfacing, at32]
curated: 2026-06-15
curated_by: config-scout
---

# DavidClawson/OpenScope-2C53T — claude-md

**Why it's worth keeping:** Includes critical technical constants like pin assignments, register addresses, and exact byte counts which prevent AI hallucinations during hardware-sensitive tasks.

**Summary:** Provides exhaustive hardware specs, memory maps, and boot procedures essential for low-level firmware development on specific MCU targets.

**Source credibility:** High; a highly detailed reverse-engineering effort with active maintenance and significant star count for its niche.

**Recency:** Current; includes modern toolchain requirements like Homebrew casks and SDL3.

**Source:** [DavidClawson/OpenScope-2C53T/CLAUDE.md](https://github.com/DavidClawson/OpenScope-2C53T/blob/6f45061fa22cb6a7f526fe7b9f4f1f3f14f4222a/CLAUDE.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FNIRSI 2C53T Open-Source Firmware Project

## What This Is

Reverse engineering and clean-room rewrite of the firmware for the **FNIRSI 2C53T**, a 3-in-1 handheld oscilloscope/multimeter/signal generator. The original firmware was decompiled from binary using Ghidra and is being refactored into clean, modular C.

## Hardware Target

- **MCU:** Artery AT32F403A — ARM Cortex-M4F @ 240MHz, 1MB flash, 224KB SRAM (with EOPB0=0xFE)
  - Originally identified as GD32F307 from firmware analysis; physical teardown revealed AT32 (markings sanded off)
  - Register-compatible with GD32/STM32F1 at the GPIO/EXMC level
- **LCD:** ST7789V 320x240 RGB565 via 16-bit parallel EXMC/XMC bus
- **FPGA:** Gowin GW1N-UV2 (non-volatile, retains bitstream across power cycles) — handles 250MS/s ADC sampling via **SPI3 data + USART2 commands**. NOTE: stock firmware nonetheless **uploads a fresh FPGA configuration over SPI3 at every boot** (the 0x3B/0x3A bulk exchange) — the NV image alone services USART meter traffic but evidently not scope capture. See `analysis_v120/h2_extracted/h2_is_gowin_bitstream_2c23t_evidence.md`.
- **SPI Flash:** Winbond W25Q128JVSQ (16MB) — UI assets and system files
- **DAC:** 2-ch
```

</details>
