---
name: malob__nix-config
source: https://github.com/malob/nix-config/blob/74642d138e671be298bd41c3258bf4a5eccf93b9/CLAUDE.md
repo: malob/nix-config
kind: claude-md
stars: 460
last_pushed: 2026-06-14T01:42:59Z
license: mit
score: 9
domains: [nix, system-administration, devops]
tags: [nix-flakes, infrastructure-as-code, automation]
curated: 2026-06-16
curated_by: config-scout
---

# malob/nix-config — claude-md

**Why it's worth keeping:** Includes highly actionable 'Common Tasks' for module creation and critical 'Gotchas' regarding PATH availability during activation scripts.

**Summary:** Explains a complex Nix flake architecture with specific build commands and symlink-based configuration patterns.

**Source credibility:** Strong; 460 stars and active maintenance indicate a high-quality, widely-used system config.

**Recency:** Very recent; includes specific instructions for Claude Code and MCP integration.

**Source:** [malob/nix-config/CLAUDE.md](https://github.com/malob/nix-config/blob/74642d138e671be298bd41c3258bf4a5eccf93b9/CLAUDE.md) · 460★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

```bash
# Build and switch to the macOS nix-darwin configuration
nh darwin switch --no-nom

# Build without switching (for testing)
nh darwin build --no-nom

# Update all flake inputs
nix flake update

# Update a specific input
nix flake update nixpkgs-unstable
```

## Architecture

This is a Nix flake that manages system configuration for macOS (via nix-darwin) and Linux (via home-manager).

### Key Structure

- **`flake.nix`** - Main entry point defining inputs, outputs, overlays, and system configurations
- **`darwin/`** - nix-darwin modules for macOS system-level configuration
- **`home/`** - home-manager modules for user-level configuration
- **`modules/`** - Reusable modules (both darwin and home-manager)
- **`lib/`** - Helper functions including `mkDarwinSystem`
- **`configs/`** - Application configs (Claude Code) symlinked for live editing
- **`overlays/`** - Nixpkgs overlays

### System Configurations

- **`darwinConfigurations.MaloBookPro`** - Primary macOS config, built with `lib.mkDarwinSystem`
- **`darwinConfigurations.githubCI`** - CI
```

</details>
