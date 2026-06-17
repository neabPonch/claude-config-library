---
name: aliyun__coolbpf
source: https://github.com/aliyun/coolbpf/blob/49733288bcf806b6c526a411ffa731ce096736b5/CLAUDE.md
repo: aliyun/coolbpf
kind: claude-md
stars: 290
last_pushed: 2026-06-13T09:50:18Z
license: mit
score: 9
domains: [systems-programming, eBPF, rust, cli-tools]
tags: [multi-language, build-orchestration, low-level]
curated: 2026-06-14
curated_by: config-scout
---

# aliyun/coolbpf — claude-md

**Why it's worth keeping:** Explains complex build patterns like the `genskel()` macro workflow and provides high-level architectural data flow diagrams that aren't obvious from code alone.

**Summary:** Provides deep technical context for a multi-language systems project involving C, Rust, and eBPF integration.

**Source credibility:** High; part of an active Alibaba Cloud repository with significant star count.

**Recency:** Current; includes modern toolchain requirements like Rust 1.80.

**Source:** [aliyun/coolbpf/CLAUDE.md](https://github.com/aliyun/coolbpf/blob/49733288bcf806b6c526a411ffa731ce096736b5/CLAUDE.md) · 290★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

coolbpf is an eBPF development platform by Alibaba Cloud that wraps libbpf for simplified BPF program development. It has three main components:

1. **libcoolbpf** (C) — Core library wrapping libbpf skeleton lifecycle (open/load/attach/destroy) with convenience macros
2. **libprofiler** (Rust) — Profiling library (perf sampling, stack symbolization, heatmap) statically linked into libcoolbpf.so
3. **AgentSight** (Rust) — Zero-instrumentation LLM agent observability tool using eBPF to capture SSL/TLS traffic and process behavior

## Build Commands

### libcoolbpf (C library)
```bash
mkdir -p build && cd build && cmake .. && make install
# With tests:   cmake -DBUILD_TESTING=on ..
# With examples: cmake -DBUILD_EXAMPLE=on ..
# Quick install: ./install.sh
# Uninstall:    ./uninstall.sh
```

CMake options: `BUILD_TESTING`, `BUILD_EXAMPLE`, `BUILD_LCC`, `ENABLE_GCOV`, `ENABLE_ASAN`, `ENABLE_PROFILE` (default ON), `ENABLE_STATIC_LINK_ELF`

### AgentSight (Rust binary)
```bash
cd src/agentsight
make build-all          # Build frontend + Rust binary
# Or
```

</details>
