---
name: tibbotech__OSS_Apps__claude
source: https://github.com/tibbotech/OSS_Apps/blob/1118ab163b904eb613ad3e80f3f42397ff937ae6/OSS_Azure/OSS_Azure_APP1/CLAUDE.md
repo: tibbotech/OSS_Apps
kind: claude-md
stars: 2
last_pushed: 2026-06-15T07:50:58Z
license: unknown
score: 9
domains: [embedded, iot, firmware]
tags: [architecture-mapping, build-system-definition, state-machine]
curated: 2026-06-15
curated_by: config-scout
---

# tibbotech/OSS_Apps — claude-md

**Why it's worth keeping:** Uses structured tables to map files to roles and explicitly defines a non-CLI build workflow to prevent tool hallucination. It also details critical state machine transitions and hardware/network fallback logic essential for agentic reasoning.

**Summary:** Provides deep domain context for a specialized embedded firmware project involving Tibbo BASIC and Azure IoT integration.

**Source credibility:** Low star count suggests this is from a niche or private industrial application rather than a widely used open-source library.

**Recency:** Current; explicitly references Claude Code and current firmware versioning patterns.

**Source:** [tibbotech/OSS_Apps/OSS_Azure/OSS_Azure_APP1/CLAUDE.md](https://github.com/tibbotech/OSS_Apps/blob/1118ab163b904eb613ad3e80f3f42397ff937ae6/OSS_Azure/OSS_Azure_APP1/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Language and Build System

This is a **Tibbo BASIC** embedded firmware project targeting the **WM2000** platform. Source files use `.tbs` (code) and `.tbh` (header/include) extensions. There is no CLI build system — compilation is performed through **Tibbo IDE**, which reads `OSS_Azure_APP1.tpr` and produces `OSS_Azure_APP1.tpc` (bytecode).

- `.tpr` — project configuration (platform, source file list, compiler settings)
- `.tpc` — compiled bytecode output (do not edit)
- `.xtxt` — descriptor files for platform libraries (settings, tables, BLE, filenum)

## Versioning

Firmware version constants are defined in `global.tbh`:
- App firmware: `AZR2.xx.xx` format (current: AZR2.09.01)
- Supervisor PIC: `OSS_SUPR_PIC_FW_xxx.hex`
- Sensor PIC: `OSS_SNS_PIC_FW_xxx.hex`

When bumping firmware versions, update constants in `global.tbh` and include the corresponding `.hex` files in the project root.

## Architecture Overview

### Entry Points and Control Flow

| File | Role |
|------|------|
| `global.tbh` | All global defines, pin assignments, library includes, firmware ve
```

</details>
