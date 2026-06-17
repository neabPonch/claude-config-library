---
name: er0080__tncattach-mercury
source: https://github.com/er0080/tncattach-mercury/blob/5d9c983d28d321962df683d788c8ee7ea9e3556e/CLAUDE.md
repo: er0080/tncattach-mercury
kind: claude-md
stars: 0
last_pushed: 2026-03-17T05:24:00Z
license: mit
score: 9
domains: [cli-tools, systems-programming, networking]
tags: [C, Linux, Protocol, Low-level]
curated: 2026-06-15
curated_by: config-scout
---

# er0080/tncattach-mercury — claude-md

**Why it's worth keeping:** Excellent use of data-flow diagrams, specific memory management constraints (no dynamic allocation), and detailed explanations of specialized protocol requirements like Mercury v2 framing.

**Summary:** Provides deep technical context for a low-level C networking tool, covering architecture, build flags, and complex protocol state machines.

**Source credibility:** The technical depth suggests a highly specialized, legitimate utility despite low GitHub visibility.

**Recency:** Very current; provides the exact type of structural context needed for modern AI agent-driven development.

**Source:** [er0080/tncattach-mercury/CLAUDE.md](https://github.com/er0080/tncattach-mercury/blob/5d9c983d28d321962df683d788c8ee7ea9e3556e/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

tncattach is a Linux utility that attaches KISS-compatible TNC (Terminal Node Controller) devices as standard Linux network interfaces (TAP or TUN). It bridges packet radio hardware to the Linux networking stack with no external dependencies beyond libc and Linux headers.

## Build Commands

```bash
make              # Build tncattach binary
make rebuild      # Clean build
make clean        # Remove compiled binary
make install      # Install to $DESTDIR/$PREFIX/bin (default: /usr/local)
make uninstall    # Remove installed files
```

Build flags: `CC=gcc`, `CFLAGS=-Wall -std=gnu11 -static-libgcc`. All five `.c` files are compiled together into a single binary.

There are no automated tests — validation is done by running the binary against actual or simulated hardware.

## Architecture

The program has a straightforward pipeline architecture:

```
Serial/TCP TNC <--KISS protocol--> [tncattach] <--/dev/net/tun--> Linux network stack
```

**Source files and their roles:**
- `tncattach.c` — Entry point, argument parsing (`argp`), main `poll()` even
```

</details>
