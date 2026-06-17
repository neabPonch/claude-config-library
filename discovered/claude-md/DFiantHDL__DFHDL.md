---
name: DFiantHDL__DFHDL
source: https://github.com/DFiantHDL/DFHDL/blob/2b6523ff720677d4d9c4a8fecad718dc7137e3e9/CLAUDE.md
repo: DFiantHDL/DFHDL
kind: claude-md
stars: 98
last_pushed: 2026-06-15T07:49:27Z
license: lgpl-3.0
score: 9
domains: [hardware-description-language, compiler-engineering, scala]
tags: [hdl, scala, compiler]
curated: 2026-06-15
curated_by: config-scout
---

# DFiantHDL/DFHDL — claude-md

**Why it's worth keeping:** Uses high-density tables to map subprojects/dependencies and includes explicit 'Claude Instructions' that integrate custom agentic skills for specialized developer workflows.

**Summary:** Provides a comprehensive technical blueprint for a complex Scala-based hardware description language, including detailed architectural hierarchies and build protocols.

**Source credibility:** High; the project is an active, sophisticated Scala 3 hardware design framework.

**Recency:** Very current; utilizes recent Scala versions and specifically prepares Claude for complex compiler-stage transformations.

**Source:** [DFiantHDL/DFHDL/CLAUDE.md](https://github.com/DFiantHDL/DFHDL/blob/2b6523ff720677d4d9c4a8fecad718dc7137e3e9/CLAUDE.md) · 98★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DFHDL — Claude Code Guide

> **For contributors and Claude Code users working on the DFHDL project.**
> This file is version-controlled — keep it updated as the project structure evolves.
> Skills for deeper topics live in [.claude/commands/](.claude/commands/).

## Project Overview

**DFHDL (DFiant HDL)** is a dataflow hardware description language embedded as a Scala 3 library. It provides timing-agnostic and device-agnostic hardware design with three levels of abstraction:

- **Dataflow (DF)**: Timing-agnostic, uses dataflow firing rules
- **Register-Transfer (RT)**: Equivalent to Chisel/Amaranth
- **Event-Driven (ED)**: Equivalent to Verilog/VHDL

Outputs: Verilog, SystemVerilog, VHDL.

## Build System

**Tool**: SBT 1.12.9 — **Scala**: 3.8.3 (nightly resolver enabled)

```bash
sbtn compile          # compile all subprojects
sbtn Test/compile     # compile all tests (separate from running them)
sbtn test             # run all unit tests
sbtn testApps         # run simulation/app tests (requires OSS CAD tools)
sbtn corePlayground   # limit test scope to core/Playground.scala only (fast iteration)
sbtn libPlayground    # limit test scope to lib/Playground.scala only (fast itera
```

</details>
