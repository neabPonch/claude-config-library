---
name: adadrag__Openclaw-Proxmox
source: https://github.com/adadrag/Openclaw-Proxmox/blob/f281a44c0f5062c2edf7f48d188934ba1934421e/CLAUDE.md
repo: adadrag/Openclaw-Proxmox
kind: claude-md
stars: 17
last_pushed: 2026-03-15T14:25:55Z
license: mit
score: 8
domains: [cli-tools, devops, infrastructure]
tags: [bash, automation, deployment]
curated: 2026-06-15
curated_by: config-scout
---

# adadrag/Openclaw-Proxmox — claude-md

**Why it's worth keeping:** The 'Architecture' section uses a step-by-step numbered list to explain complex logic flow, while 'Development Notes' captures critical edge cases like in-place sed patches and specific user account restrictions.

**Summary:** Provides a high-density breakdown of a single-script deployment tool's procedural execution flow and system requirements.

**Source credibility:** Moderate; based on a functional niche tool with active maintenance.

**Recency:** Current; references Proxmox 8.x and Debian 13.

**Source:** [adadrag/Openclaw-Proxmox/CLAUDE.md](https://github.com/adadrag/Openclaw-Proxmox/blob/f281a44c0f5062c2edf7f48d188934ba1934421e/CLAUDE.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OpenClaw on Proxmox is a single-script deployment tool (`setup-openclaw-lxc.sh`) that automates creating a Proxmox LXC container with a fully configured OpenClaw AI assistant, LXQt desktop, Google Chrome, and VNC/noVNC remote access. It targets Proxmox VE 8.x+ hosts running as root.

## Architecture

The entire project is one ~460-line Bash script with this flow:

1. **Pre-flight** — Verify Proxmox CLI tools (`pct`, `pvesh`, `pveam`) and root access
2. **User prompts** — Collect container password, disk/memory/CPU/resolution settings
3. **Auto-detection** — Find next VMID and storage backends via `pvesh` JSON + Python parsing
4. **Template management** — Download Debian 13 template if missing
5. **Container creation** — Privileged LXC, DHCP networking
6. **Package installation** — Node.js 22, Homebrew (as non-root `brewuser`), OpenClaw (npm global), LXQt, TigerVNC, noVNC, Google Chrome, OpenClaw browser extension
7. **Configuration** — OpenClaw gateway settings, VNC password/xstartup, noVNC auto-scaling patch, Chrome as default browser
8. **Deskt
```

</details>
