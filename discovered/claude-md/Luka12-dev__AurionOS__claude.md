---
name: Luka12-dev__AurionOS__claude
source: https://github.com/Luka12-dev/AurionOS/blob/eb0ea07e81632b6d0b76d69a08d5634bf5c36d6a/.claude/CLAUDE.md
repo: Luka12-dev/AurionOS
kind: claude-md
stars: 35
last_pushed: 2026-05-01T13:11:56Z
license: mit
score: 9
domains: [systems-programming, os-dev]
tags: [x86, assembly, c, kernel]
curated: 2026-06-15
curated_by: config-scout
---

# Luka12-dev/AurionOS — claude-md

**Why it's worth keeping:** Includes high-value 'Good vs Bad' code style examples and detailed hardware-level structural knowledge necessary for debugging non-standard environments.

**Summary:** Provides essential low-level architectural context, memory maps, and specific build/debug workflows for a custom x86 operating system.

**Source credibility:** Niche hobbyist project with reasonable social proof (35 stars).

**Recency:** Very recent; last pushed 1 month ago.

**Source:** [Luka12-dev/AurionOS/.claude/CLAUDE.md](https://github.com/Luka12-dev/AurionOS/blob/eb0ea07e81632b6d0b76d69a08d5634bf5c36d6a/.claude/CLAUDE.md) · 35★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AurionOS - Claude Development Guide

This document provides context and guidance for working with the AurionOS codebase. AurionOS is a complete operating system built from scratch in x86 assembly and C - no Linux kernel, no POSIX, no borrowed code.

---

## Project Overview

AurionOS is a modern, bootable operating system featuring:

- Custom bootloader and kernel written in x86 assembly
- Desktop environment with windowed GUI
- Dual-mode operation (GUI and DOS modes)
- Custom filesystem with persistence
- Network stack (TCP/IP, DHCP, HTTP/HTTPS)
- Built-in applications (browser, terminal, paint, calculator, games)
- AurionGL 3D graphics library (software rasterization)
- Blaze browser engine (HTML/CSS/JavaScript)

**Target**: Real hardware and virtual machines (QEMU, VMware, VirtualBox)
**Architecture**: x86 32-bit protected mode
**Language**: Assembly (NASM) + C11 (freestanding)

---

## Build System

### Platform Detection

The Makefile automatically detects the platform:
- **Windows**: Native Windows build (rarely used)
- **WSL2**: Linux tools with Windows QEMU for CD-ROM (avoids QEMU 8.2.2 crash)
- **Linux**: Native Linux build

### Build Commands

```bash
# Standard build (
```

</details>
