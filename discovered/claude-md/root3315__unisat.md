---
name: root3315__unisat
source: https://github.com/root3315/unisat/blob/79b911706470251b824021f65e66f53d81d5232d/CLAUDE.md
repo: root3315/unisat
kind: claude-md
stars: 3
last_pushed: 2026-04-30T10:09:16Z
license: apache-2.0
score: 10
domains: [embedded-systems, aerospace, firmware, systems-programming]
tags: [architecture-rules, cross-language-parity, hardware-interfacing, verification-driven]
curated: 2026-06-15
curated_by: config-scout
---

# root3315/unisat — claude-md

**Why it's worth keeping:** Uses 'rules of engagement' to prevent architectural violations (e.g., layer encapsulation) and explains the exact sequence required to add new form factors across multiple files. It also provides specific instructions for maintaining cross-language protocol parity via golden vectors.

**Summary:** Provides high-density technical context for a multi-language embedded system involving C firmware and Python mission control.

**Source credibility:** High; reflects a complex, high-integrity engineering project with rigorous testing and hardware constraints.

**Recency:** Current; integrates modern toolchain requirements and specific Claude Code navigation patterns.

**Source:** [root3315/unisat/CLAUDE.md](https://github.com/root3315/unisat/blob/79b911706470251b824021f65e66f53d81d5232d/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

**UniSat** — universal modular satellite software platform. **v1.3.0** extended support from CubeSat-only to a multi-class registry (CanSat minimal/standard/advanced, CubeSat 1U/1.5U/2U/3U/6U/12U, suborbital rocket, HAB, drone, rover, custom). **v1.3.1** wired the configurator into the registry and shipped a full operations guide. TRL-5-hardened on the CubeSat-3U reference profile. Three cooperating codebases share one repo and one on-air protocol stack:

- **`firmware/`** — STM32F446RE OBC firmware in C11 + FreeRTOS (host-buildable for tests; cross-compiles to `.elf/.bin/.hex` when `arm-none-eabi-gcc` is on PATH).
- **`flight-software/`** — Python 3.11 asyncio mission controller meant to run on a Raspberry Pi Zero 2 W, talking to the OBC over UART.
- **`ground-station/`** — Streamlit dashboard + AX.25 CLI tooling (`cli/ax25_listen`, `cli/ax25_send`).

Plus: `simulation/` (orbit/power/thermal/link Python sims), `configurator/` (Streamlit mission builder), `payloads/` (plugin templates), `hardware/` (KiCad + BOM), `docs/` (SRS, ADRs, threat model, trace ma
```

</details>
