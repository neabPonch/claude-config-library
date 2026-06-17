---
name: kottlerg__seraph-i686
source: https://github.com/kottlerg/seraph-i686/blob/7daed742bbd78b09335d2da580d51c203438b1ea/CLAUDE.md
repo: kottlerg/seraph-i686
kind: claude-md
stars: 1
last_pushed: 2026-02-17T14:11:35Z
license: gpl-3.0
score: 8
domains: [systems, os-development]
tags: [x86, kernel, c, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# kottlerg/seraph-i686 — claude-md

**Why it's worth keeping:** It explicitly defines the project dependency order and provides vital memory mapping/entry point information essential for systems programming assistance.

**Summary:** Provides critical low-level architectural context, toolchain specifications, and build orchestration details for a custom x86 operating system.

**Source credibility:** Niche hobbyist OS project; low stars but high technical density.

**Recency:** Very recent, highly relevant to current development workflows.

**Source:** [kottlerg/seraph-i686/CLAUDE.md](https://github.com/kottlerg/seraph-i686/blob/7daed742bbd78b09335d2da580d51c203438b1ea/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Seraph is a Unix-like operating system kernel written from scratch in C and x86 assembly, targeting i386 with GRUB Multiboot boot. It includes a custom GCC/binutils toolchain (i686-seraph), a POSIX-compatible C library (libc), a dynamic linker, and userspace utilities.

See @docs/usage.md for build requirements and debug/cleanup commands. See @docs/architecture.md for the full project layout and subsystem details.

## Build Details

Build order is defined in `script/config.sh` via the PROJECTS variable: libc, kernel, linker, lib, bin. Each project has its own Makefile. The toolchain cross-compiler and sysroot paths are configured in `script/config.sh`. Host tool differences (e.g., `grub-file` vs `grub2-file` on Fedora) are auto-detected there too.

Project should always be built and cleaned up by the scripts such as `build.sh`, `mkiso.sh`, `clean.sh`, etc.

CI runs via GitHub Actions (`.github/workflows/CI.yml`) using a Docker image with the pre-built toolchain. It builds and produces a `seraph.iso` artifact.

## Architecture

The kernel is a mon
```

</details>
