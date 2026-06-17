---
name: jwiegley__nix-config__claude
source: https://github.com/jwiegley/nix-config/blob/ecc8f308813cc9fa32141eae543c2bf9b40a5d94/docs/CLAUDE.md
repo: jwiegley/nix-config
kind: claude-md
stars: 460
last_pushed: 2026-06-12T16:35:29Z
license: unknown
score: 9
domains: [devops, system-administration, nix, infrastructure]
tags: [nix, multihost, environment-context, infrastructure-as-code]
curated: 2026-06-15
curated_by: config-scout
---

# jwiegley/nix-config — claude-md

**Why it's worth keeping:** The 'Managed Machines' table is a masterclass in providing context for distributed environments; it also includes explicit instructions for using specialized subagents and slash commands.

**Summary:** This file maps out a complex, multi-host Nix configuration ecosystem, providing precise rebuild commands and environment details for every machine.

**Source credibility:** High-quality personal configuration with significant social proof (460 stars) and active maintenance.

**Recency:** Highly current, specifically referencing modern Claude Code features like MCP servers and subagents.

**Source:** [jwiegley/nix-config/docs/CLAUDE.md](https://github.com/jwiegley/nix-config/blob/ecc8f308813cc9fa32141eae543c2bf9b40a5d94/docs/CLAUDE.md) · 460★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a personal Nix configuration repository for managing macOS (Darwin), NixOS, and Ubuntu systems using Nix flakes, nix-darwin, and home-manager. The shared user environment in `config/johnw.nix` and `config/packages.nix` is used across all five machines below.

## Managed Machines

| Host | OS | Arch | User | Home | Nix binary | rsync binary | Config location | Rebuild command |
|------|----|------|------|------|-----------|-------------|-----------------|----------------|
| **hera** | macOS | aarch64-darwin | `johnw` | `/Users/johnw` | `/nix/var/nix/profiles/default/bin/nix` | `/etc/profiles/per-user/johnw/bin/rsync` | `~/src/nix` (this repo) | `u switch` |
| **clio** | macOS | aarch64-darwin | `johnw` | `/Users/johnw` | `/nix/var/nix/profiles/default/bin/nix` | `/etc/profiles/per-user/johnw/bin/rsync` | `~/src/nix` (this repo) | `u switch` |
| **vulcan** | NixOS (Asahi Linux) | aarch64-linux | `johnw` | `/Users/johnw` | `/run/current-system/sw/bin/nix` | `/etc/profiles/per-user/johnw/bin/rsync` | `/etc/nixos` | `sudo nixos-rebuild switch --flake
```

</details>
