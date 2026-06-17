---
name: aaronsbrown__fpga_8-Bit_SAP-2.0
source: https://github.com/aaronsbrown/fpga_8-Bit_SAP-2.0/blob/6241122a3af12349b00f6e1f1f36b5ad5afcd948/CLAUDE.md
repo: aaronsbrown/fpga_8-Bit_SAP-2.0
kind: claude-md
stars: 0
last_pushed: 2025-06-15T01:44:10Z
license: unknown
score: 9
domains: [hardware, embedded-systems, cli-tools]
tags: [fpga, cpu-architecture, anchor-comments, guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# aaronsbrown/fpga_8-Bit_SAP-2.0 — claude-md

**Why it's worth keeping:** The `AIDEV-` anchor system is a brilliant technique for persistent knowledge; the scale-based guardrails (LOC/file counts) are essential for controlling agentic refactoring.

**Summary:** A highly specialized configuration for a hardware project that uses unique 'anchor comment' patterns to maintain AI context across sessions.

**Source credibility:** Low social proof (0 stars), but the high density of specific technical instructions suggests a highly competent author.

**Recency:** Very current, explicitly referencing Claude Code and modern Python standards.

**Source:** [aaronsbrown/fpga_8-Bit_SAP-2.0/CLAUDE.md](https://github.com/aaronsbrown/fpga_8-Bit_SAP-2.0/blob/6241122a3af12349b00f6e1f1f36b5ad5afcd948/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an FPGA-based 8-bit CPU project implementing a custom SAP2-style computer with 16-bit addressing. The project includes:

- Custom CPU with ALU, control unit, and registers
  - Supports compile time configuration of reset behavior, choosing from:
  - Static reset vector (ROM start = F000); default setting
  - Dynamic reset vector table at FFFC/FFFD (modeled on 6502)
- Custom ISA (see docs/hardware/0_ISA.md; please note unconventional MOV instruction (Src => Dest)
- Memory-mapped I/O (MMIO) infrastructure (see docs/hardware/1_memory_map.md)
- UART peripheral for serial communication (see docs/hardware/2_uart_datasheet.md))
- Complete custom assembler toolchain for the custom instruction set
- Comprehensive test suite with simulation infrastructure, support by continuous integration workflow on github
- Robust dev tools in scripts/

## Targeted Hardware

— Alchitry Cu FPGA development board V2 (<https://shop.alchitry.com/products/alchitry-cu-v2>)
— ICE40HX8K-CB132 FPGA (<https://www.latticesemi.com/ice40>)
— **Note**: Project supports both C
```

</details>
