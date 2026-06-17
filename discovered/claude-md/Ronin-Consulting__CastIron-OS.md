---
name: Ronin-Consulting__CastIron-OS
source: https://github.com/Ronin-Consulting/CastIron-OS/blob/897b34fdbd4efac7073b91d8d6c8b151075935a3/CLAUDE.md
repo: Ronin-Consulting/CastIron-OS
kind: claude-md
stars: 0
last_pushed: 2026-03-09T14:25:41Z
license: unknown
score: 9
domains: [embedded-linux, systems-programming, devops]
tags: [buildroot, linux-distro, cross-compilation, systemd]
curated: 2026-06-14
curated_by: config-scout
---

# Ronin-Consulting/CastIron-OS — claude-md

**Why it's worth keeping:** Includes crucial 'gotchas' like specific Makefile indentation rules, detailed build pipeline side-effects, and standalone development workflows that prevent the AI from breaking the cross-compilation logic.

**Summary:** Provides deep technical context for a custom Linux distribution build process involving Buildroot, hardware-specific targets, and complex filesystem orchestration.

**Source credibility:** While the repo has low social proof (0 stars), the extreme technical specificity indicates a high-quality, functional project.

**Recency:** Modern; incorporates contemporary tools like Bun and standard Buildroot/Systemd workflows.

**Source:** [Ronin-Consulting/CastIron-OS/CLAUDE.md](https://github.com/Ronin-Consulting/CastIron-OS/blob/897b34fdbd4efac7073b91d8d6c8b151075935a3/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

CastIron-OS is a minimal, security-hardened Linux distribution that runs FRIDAY — a Bun TypeScript AI personal assistant. Built with Buildroot as a custom `br2-external` tree. Targets x86_64 and ARM64 (Raspberry Pi 4B/5). The OS boots into a surf (WebKitGTK) kiosk displaying FRIDAY's web UI on port 3000, with ttyd providing a browser-based terminal on port 7681 and xterm available via openbox.

## Build Commands

Builds require a **Linux host** with: make, gcc, g++, git, unzip, wget, rsync, cpio, python3, bun.

```bash
make setup              # Init Buildroot submodule, check host deps
make x86_64             # Full x86_64 build (~1-2 hours first time)
make aarch64            # Full ARM64 build
make qemu               # Build x86_64 + boot ISO in QEMU (needs qemu-system-x86_64)
make qemu-serial        # Build x86_64 + boot ISO in QEMU (serial console, no GUI)
make agent-rebuild      # Quick: rebuild Bun package + regenerate image
make menuconfig         # Buildroot menuconfig (load defconfig first)
make linux-menuconfig   # Kernel menuconfig
make sav
```

</details>
