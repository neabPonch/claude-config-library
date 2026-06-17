---
name: Windscribe__Desktop-App
source: https://github.com/Windscribe/Desktop-App/blob/c6d51c4eaf061f7a0de9713428b80be7706cec46/CLAUDE.md
repo: Windscribe/Desktop-App
kind: claude-md
stars: 993
last_pushed: 2026-06-08T17:21:06Z
license: gpl-2.0
score: 9
domains: [desktop-app, security, cpp, cross-platform]
tags: [architectural-map, system-level, qt-framework]
curated: 2026-06-15
curated_by: config-scout
---

# Windscribe/Desktop-App — claude-md

**Why it's worth keeping:** It maps functional logic to specific directory structures and documents critical cross-platform naming conventions essential for navigating system-level code.

**Summary:** Acts as a high-density architectural roadmap for a complex, multi-platform C++ VPN client.

**Source credibility:** High; originates from a popular (993 stars), actively maintained production-grade repository.

**Recency:** Extremely current, with updates within the last month.

**Source:** [Windscribe/Desktop-App/CLAUDE.md](https://github.com/Windscribe/Desktop-App/blob/c6d51c4eaf061f7a0de9713428b80be7706cec46/CLAUDE.md) · 993★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Windscribe Desktop VPN** - A production-grade, cross-platform VPN client for Windows, macOS, and Linux written in C++17 with Qt.

### What It Does

This application provides secure, private internet access by routing your traffic through encrypted VPN tunnels. It protects your physical location, blocks ads and trackers, prevents DNS leaks, and helps bypass censorship through multiple connection strategies.

**Current Version**: 2.21.1 (guinea pig build - see `src/client/client-common/version/windscribe_version.h`)

**Supported Platforms**:
- Windows 10/11 (amd64, arm64), Windows Server 2022
- macOS 13+ (amd64, arm64)
- Ubuntu 22.04+, Fedora 36+, openSUSE Leap 15.6, Arch, immutable distros (amd64, arm64)

### Key Features

- **Multiple VPN Protocols**: WireGuard (with Post-Quantum encryption), OpenVPN (UDP/TCP), IKEv2, Stealth, WSTunnel - over 20 connection ports
- **Privacy & Security**: Always-on firewall eliminates leaks, MAC address spoofing, DNS-based content filtering (R.O.B.E.R.T.), custom DNS support
- **Advanced Networking**: Network-wi
```

</details>
