---
name: dustinlyons__nixos-config
source: https://github.com/dustinlyons/nixos-config/blob/9022b2b3b1573c9ab4d666e1feb1a81bd81135d3/CLAUDE.md
repo: dustinlyons/nixos-config
kind: claude-md
stars: 3538
last_pushed: 2026-06-11T13:18:20Z
license: bsd-3-clause
score: 9
domains: [devops, infrastructure-as-code, cli-tools]
tags: [nix, nixos, macos, configuration-management]
curated: 2026-06-15
curated_by: config-scout
---

# dustinlyons/nixos-config — claude-md

**Why it's worth keeping:** It includes critical 'gotchas' like the Git tracking requirement for flakes and provides specific workflow instructions for complex sub-systems like Emacs and package placement.

**Summary:** A highly detailed configuration guide for a cross-platform NixOS and macOS environment using Nix Flakes.

**Source credibility:** Highly credible; high star count, active maintenance, and technically dense documentation.

**Recency:** Very current; mentions modern software like KDE Plasma 6 and follows up-to-date Nix patterns.

**Source:** [dustinlyons/nixos-config/CLAUDE.md](https://github.com/dustinlyons/nixos-config/blob/9022b2b3b1573c9ab4d666e1feb1a81bd81135d3/CLAUDE.md) · 3538★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a cross-platform NixOS configuration repository supporting both macOS (via nix-darwin) and NixOS systems. It uses Nix Flakes exclusively and follows a modular architecture.

## System Environment

- **Display Server**: Wayland (not X11)
- **Desktop Environment**: KDE Plasma 6
- **Window Manager**: KWin (Wayland)

Important: When working with GUI applications, ensure Wayland compatibility. For example:
- Use `rofi-wayland` instead of `rofi`
- Check for Wayland-specific versions of applications
- Some X11-only applications may need XWayland compatibility layer

## Key Commands

### Building and Switching Configurations

**NixOS (x86_64-linux):**
```bash
# Build and switch to new configuration
nix run .#build-switch

# Build, switch, and restart Emacs daemon (use after Emacs config changes)
nix run .#build-switch-emacs

# Install fresh system (without secrets)
nix run .#install

# Install fresh system (with secrets)
nix run .#install-with-secrets

# Clean up old generations and boot files (frees disk space)
nix run .#clean
```

**Importan
```

</details>
