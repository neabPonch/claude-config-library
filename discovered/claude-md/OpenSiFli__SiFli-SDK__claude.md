---
name: OpenSiFli__SiFli-SDK__claude
source: https://github.com/OpenSiFli/SiFli-SDK/blob/8494c1ccb425ebb08f0b3935031552a6df869079/.claude/CLAUDE.md
repo: OpenSiFli/SiFli-SDK
kind: claude-md
stars: 168
last_pushed: 2026-06-13T23:04:31Z
license: apache-2.0
score: 8
domains: [embedded, firmware, c]
tags: [build-system, rtos, scons]
curated: 2026-06-14
curated_by: config-scout
---

# OpenSiFli/SiFli-SDK — claude-md

**Why it's worth keeping:** Includes specific shell/PowerShell initialization commands and explains complex multi-core (HCPU/LCPU) project structures that a tool needs to understand.

**Summary:** Provides exhaustive build system instructions, environment setup requirements, and hardware abstraction layers for an embedded SDK.

**Source credibility:** Active industry SDK with consistent maintenance and growing popularity in its niche.

**Recency:** Highly relevant for modern agentic workflows requiring environment setup before execution.

**Source:** [OpenSiFli/SiFli-SDK/.claude/CLAUDE.md](https://github.com/OpenSiFli/SiFli-SDK/blob/8494c1ccb425ebb08f0b3935031552a6df869079/.claude/CLAUDE.md) · 168★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SiFliSDK

This file provides guidance to agents when working with code in this repository.

## Overview

SiFli SDK is an embedded firmware development framework built on RT-Thread RTOS, targeting SiFli Technologies' SoC family. The SDK supports five chip families: SF32LB52X, SF32LB55X, SF32LB56X, SF32LB57X, and SF32LB58X, with some supporting multi-core configurations (HCPU, LCPU and ACPU).

## Build System

The build system uses **SCons** with **Kconfig** for configuration. All builds must run inside a properly initialized environment.

### Environment Setup (Windows PowerShell)

```powershell
./export.ps1
```

### Environment Setup (Linux/macOS)

```bash
source ./export.sh
```

### Building a Project

Navigate to an example's project directory which contains file `SConstruct` and `proj.conf`, then:

#### Build for a specific board
```
scons --board=<board_name> -j8
```
The artifacts are generated under directory `build_<board_name>`. 

#### Interactive configuration menu

```bash
sdk.py menuconfig --board=<board_name>
```

Example board names: `eh-lb551_hcpu`, `eh-lb563_hcpu`, `ec-lb583_hcpu`, `sf32lb52-lcd_n16r8_hcpu` for HCPU core.


### Configure a Board
Navigate to a board
```

</details>
