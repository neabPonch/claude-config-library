---
name: oxidecomputer__quartz
source: https://github.com/oxidecomputer/quartz/blob/6f68cc720f900e2fddd1cb156ef4cd99bcad4238/CLAUDE.md
repo: oxidecomputer/quartz
kind: claude-md
stars: 22
last_pushed: 2026-06-12T14:05:11Z
license: unknown
score: 9
domains: [hardware-design, hdl, embedded-systems, fpga]
tags: [vhdl, bsv, buck2, vunit, hardware-abstraction]
curated: 2026-06-15
curated_by: config-scout
---

# oxidecomputer/quartz — claude-md

**Why it's worth keeping:** Provides exact commands for refreshing LSP/RDL dependencies and includes specific code templates for the VUnit testbench structure which prevents LLM hallucinations about boilerplate.

**Summary:** A detailed guide for hardware development including build systems (Buck2), LSP configuration, and VUnit testing frameworks.

**Source credibility:** High; from a specialized hardware company (Oxide Computer) with active maintenance.

**Recency:** Extremely current, reflecting modern Buck2 workflows and recent repository activity.

**Source:** [oxidecomputer/quartz/CLAUDE.md](https://github.com/oxidecomputer/quartz/blob/6f68cc720f900e2fddd1cb156ef4cd99bcad4238/CLAUDE.md) · 22★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Quartz is a collection of soft-logic designs and hardware abstraction libraries (HALs) for various subsystems found in Oxide hardware. This includes components such as Ignition, power sequencing for system boards, and QSFP interface management.

## Build System

Quartz uses two build systems in parallel:

### Buck2 (Primary/Modern)
- Used for VHDL, BSV, and RDL flows
- Supports VUnit simulations for VHDL and Bluesim for BSV
- Supports Xilinx FPGA toolchain integration
- Supports Lattice FPGAs via Yosys and GDHL VHDL plugin

#### Prerequisites
- Buck2 installed: `cargo +nightly-2024-10-13 install --git https://github.com/facebook/buck2.git --tag "2025-02-01" buck2`
- Python 3.10+ with packages: `pip install -r tools/requirements.txt`
- NVC simulator (minimum version 1.13.1)
- Vivado on PATH for Xilinx designs

#### Key Commands
- `buck2 ctargets /...` - List all available targets
- `buck2 run <target>` - Run a simulation
- `buck2 bxl //tools/vunit-sims.bxl:vunit_sim_gen` - List all simulation testbenches
- `buck2 run //tools/multitool:multitool --
```

</details>
