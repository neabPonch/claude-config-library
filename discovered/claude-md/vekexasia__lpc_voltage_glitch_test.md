---
name: vekexasia__lpc_voltage_glitch_test
source: https://github.com/vekexasia/lpc_voltage_glitch_test/blob/72ff061455bc9c19634b06a76693a17dd9710f50/claude.md
repo: vekexasia/lpc_voltage_glitch_test
kind: claude-md
stars: 6
last_pushed: 2026-03-21T19:22:21Z
license: unknown
score: 8
domains: [embedded, security, hardware]
tags: [ARM, C, glitching, microcontroller]
curated: 2026-06-15
curated_by: config-scout
---

# vekexasia/lpc_voltage_glitch_test — claude-md

**Why it's worth keeping:** Provides critical low-level constraints such as specific compiler optimization requirements (O0) and strict GPIO definition conventions essential for embedded-target accuracy.

**Summary:** Technical specification for a hardware voltage glitching testbed targeting NXP LPC1768 and RP2040 microcontrollers.

**Source credibility:** High; contains highly specific hardware/register details consistent with a real engineering project.

**Recency:** Current; uses modern Dockerized build workflows and ARM toolchains.

**Source:** [vekexasia/lpc_voltage_glitch_test/claude.md](https://github.com/vekexasia/lpc_voltage_glitch_test/blob/72ff061455bc9c19634b06a76693a17dd9710f50/claude.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# LPC Voltage Glitch Test

## Project Overview

Hardware voltage glitching attack testbed targeting an **NXP LPC1768** (ARM Cortex-M3) microcontroller. A **Raspberry Pi Pico (RP2040)** acts as the glitch controller, driving a **MAX4619** analog multiplexer to momentarily drop the LPC's VCC to GND at precise timing, attempting to corrupt the CPU's execution (e.g., bypass CRP code-read protection or corrupt loop counters).

## Architecture

```
LPC1768 (target)  <--VCC via MAX4619-->  RP2040 (controller)
  P0.10 (signal) -----> GPIO 11
                         GPIO 18 → MAX EN
                         GPIO 19 → MAX A/B/C select
```

- **`lpc/`** — Target firmware (bare-metal C, ARM Cortex-M3). Runs a triple-nested loop summing to 1,000,000, toggles P0.10 as a trigger signal, reports glitch success via UART.
- **`glitcher/`** — Controller firmware (RP2040 C SDK + PIO). Uses DMA + PIO to bit-bang a glitch pattern on the MAX4619 selector pin at system clock speed. Waits for the LPC signal pin before firing.
- **`pico-sdk/`** — Git submodule (Raspberry Pi Pico SDK).

## Key Files

| File | Purpose |
|---|---|
| `lpc/main.c` | Target firmware — loop, signal pin, UART output, CRP word, BOD
```

</details>
