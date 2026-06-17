---
name: patrickjaja__claude-cowork-service
source: https://github.com/patrickjaja/claude-cowork-service/blob/6691f926d58e744be06b86c98142b4d022ad575b/CLAUDE.md
repo: patrickjaja/claude-cowork-service
kind: claude-md
stars: 159
last_pushed: 2026-06-12T00:16:40Z
license: mit
score: 10
domains: [systems-programming, reverse-engineering, go]
tags: [system-daemon, binary-analysis, protocol-verification]
curated: 2026-06-15
curated_by: config-scout
---

# patrickjaja/claude-cowork-service — claude-md

**Why it's worth keeping:** It provides exact shell commands for deep-dive investigation (reverse engineering) and explicitly maps 'fragile' files to external update triggers, enabling the AI to act as a proactive maintainer rather than just a coder.

**Summary:** A high-density guide for maintaining a fragile, reverse-engineered system by documenting specific verification workflows and binary analysis steps.

**Source credibility:** High; very recently updated and focuses on a highly specialized technical niche.

**Recency:** Extremely current; demonstrates advanced usage of LLM capabilities for system-level investigation.

**Source:** [patrickjaja/claude-cowork-service/CLAUDE.md](https://github.com/patrickjaja/claude-cowork-service/blob/6691f926d58e744be06b86c98142b4d022ad575b/CLAUDE.md) · 159★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Project Guidelines

## Project Overview

This is a native Linux backend daemon for Claude Desktop's Cowork feature. It reverse-engineers the Windows `cowork-svc.exe` (Go/Hyper-V) and implements the same JSON-over-Unix-socket protocol, but executes directly on the host (no VM).

**Language:** Pure Go, zero external dependencies (stdlib only).

**Binary:** `cowork-svc-linux`

**Socket:** `$XDG_RUNTIME_DIR/cowork-vm-service.sock` (falls back to `/tmp/` if `$XDG_RUNTIME_DIR` is unset).

**Session dirs:** `~/.local/share/claude-cowork/sessions/<name>/`

**Protocol:** 21 active RPC methods (1 removed) over length-prefixed JSON (4-byte big-endian header, max 10 MB per message).

**Key constraint:** The upstream binary (`cowork-svc.exe`) is managed remotely by Anthropic and changes without notice. Every RPC method, parameter name, and protocol behavior can change between releases. This makes the project inherently fragile --- protocol documentation and handler code must be re-validated on each upstream update.

## Build & Run

```bash
# Build
make build

# Build for ARM64
make build-arm64

# Install (binary + systemd service)
sudo make install

# Run manually in debug mode
co
```

</details>
