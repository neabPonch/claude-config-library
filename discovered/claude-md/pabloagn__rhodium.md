---
name: pabloagn__rhodium
source: https://github.com/pabloagn/rhodium/blob/c76517255191302a9a6a8e7cb0c030a521abb801/CLAUDE.md
repo: pabloagn/rhodium
kind: claude-md
stars: 97
last_pushed: 2026-03-27T15:07:51Z
license: gpl-3.0
score: 9
domains: [nixos, devops, infrastructure-as-code]
tags: [nix, just, system-config, modular]
curated: 2026-06-15
curated_by: config-scout
---

# pabloagn/rhodium — claude-md

**Why it's worth keeping:** Includes prescriptive development workflows (recipes) for common tasks and categorizes command-line operations to enable autonomous system management via `just` commands.

**Summary:** Maps out a hyper-modular NixOS architecture, detailing data-logic separation and specialized argument flows.

**Source credibility:** Strong; 97 stars indicates a respected community project with recent maintenance history.

**Recency:** Very current; reflects modern Nix/Flake patterns used in today's development environments.

**Source:** [pabloagn/rhodium/CLAUDE.md](https://github.com/pabloagn/rhodium/blob/c76517255191302a9a6a8e7cb0c030a521abb801/CLAUDE.md) · 97★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Rhodium is a hypermodular, declarative NixOS system built using Nix flakes. It combines system-level configuration with Home Manager for user-specific configurations, using a profile-based approach for 150+ curated packages. The architecture separates concerns between hosts, users, modules, and data.

## Architecture

### Core Structure

- **`flake.nix`**: Main entry point defining all inputs, outputs, and NixOS configurations
- **`hosts/`**: Per-host NixOS system configurations (e.g., `host_001/`, `host_002/`)
- **`users/`**: Per-user Home Manager configurations (e.g., `user_001/`)
- **`modules/`**: System-level NixOS modules organized by category (boot, desktop, hardware, security, services, etc.)
- **`home/`**: User-level Home Manager modules (apps, desktop, development, environment, shells, etc.)
- **`data/`**: Declarative user and host data separated from logic
  - `data/users/users.nix`: User account definitions
  - `data/hosts/hosts.nix`: Host metadata (hostname, monitor config, etc.)
  - `data/users/preferences/`: User preferences (apps, behavior
```

</details>
