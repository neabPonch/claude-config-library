---
name: chili-chips-ba__wireguard-fpga__claude
source: https://github.com/chili-chips-ba/wireguard-fpga/blob/002c8f12fd34d8bbfe7a790c058c8c0a3219651c/3.build/pipelinec_build/CLAUDE.md
repo: chili-chips-ba/wireguard-fpga
kind: claude-md
stars: 1334
last_pushed: 2026-05-23T04:43:33Z
license: bsd-3-clause
score: 9
domains: [hardware-design, embedded-systems, security]
tags: [hls, fpga, verilog, wireguard]
curated: 2026-06-15
curated_by: config-scout
---

# chili-chips-ba/wireguard-fpga — claude-md

**Why it's worth keeping:** Includes essential domain-specific patterns like unique module instantiation via #define/#include and simulation macros that prevent AI from using standard C logic in a hardware context.

**Summary:** Provides critical architectural data flows and specific toolchain pragmas required for the PipelineC HLS workflow.

**Source credibility:** High; high star count (1300+) and active maintenance on specialized security/hardware software.

**Recency:** Current; provides highly specific technical constraints relevant to modern HLS-based FPGA development.

**Source:** [chili-chips-ba/wireguard-fpga/3.build/pipelinec_build/CLAUDE.md](https://github.com/chili-chips-ba/wireguard-fpga/blob/002c8f12fd34d8bbfe7a790c058c8c0a3219651c/3.build/pipelinec_build/CLAUDE.md) · 1334★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This directory contains the **PipelineC** HLS (High-Level Synthesis) implementation of ChaCha20-Poly1305 AEAD encryption/decryption for the Wireguard FPGA project. It targets an Artix-7 xc7a200tffg1156-2 FPGA at 80 MHz.

PipelineC compiles C source files directly into synthesizable Verilog. The `$PIPELINEC` environment variable must point to the PipelineC executable before running any build script.

## Build Commands

All build scripts clear their output directory and regenerate from scratch.

**Generate Verilog (for FPGA synthesis):**
```bash
./build_verilog.sh          # Standalone encrypt → generated-files-verilog/
./build_verilog_decrypt.sh  # Standalone decrypt → generated-files-verilog-decrypt/
./build_verilog_shared.sh   # Shared encrypt+decrypt → generated-files-verilog-shared/
```

**Simulate with cocotb + GHDL:**
```bash
./build_sim_comb.sh         # Combinational sim, encrypt TB (100 steps)
./build_sim_pipe.sh         # Pipelined sim, encrypt TB (150 steps)
./build_sim_comb_dec.sh     # Combinational sim, decrypt TB
./build_sim_pipe_de
```

</details>
