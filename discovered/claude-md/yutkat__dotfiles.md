---
name: yutkat__dotfiles
source: https://github.com/yutkat/dotfiles/blob/35fbcc08b67a41b3567c48305375a3673b3dd981/CLAUDE.md
repo: yutkat/dotfiles
kind: claude-md
stars: 963
last_pushed: 2026-06-13T08:35:19Z
license: mit
score: 9
domains: [cli-tools, devops, system-config]
tags: [nix, dotfiles, shell, linux]
curated: 2026-06-15
curated_by: config-scout
---

# yutkat/dotfiles — claude-md

**Why it's worth keeping:** It includes specific verification commands (nix flake check, linting) and clarifies the symlink architecture which is critical for preventing destructive file operations in Nix environments.

**Summary:** Explains a complex NixOS/Home Manager flake-based configuration with multi-host support. It provides clear paths for applying and verifying system changes.

**Source credibility:** High; a highly starred, actively maintained repository from a specialized user.

**Recency:** Current; explicitly mentions Claude Code usage.

**Source:** [yutkat/dotfiles/CLAUDE.md](https://github.com/yutkat/dotfiles/blob/35fbcc08b67a41b3567c48305375a3673b3dd981/CLAUDE.md) · 963★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Architecture Overview

This is a comprehensive dotfiles repository for NixOS/Nix systems with multi-host support:

- **Flake-based configuration**: Uses `flake.nix` with host-specific configurations
- **Multi-host support**: Supports both NixOS systems and standalone Home Manager installations
- **Modular structure**: Separate CLI and GUI configurations in home-manager/
- **Host-specific configs**: Per-host overrides in nixos/hosts/ and home-manager/hosts/
- **Environment variable support**: NIX_USERNAME and NIX_DOTFILES_PATH for customization
- **Symlink management**: Uses `mkOutOfStoreSymlink` for live-editable configurations

### Key Configuration Files

- `flake.nix`: Main configuration defining hosts and build functions
- `home.nix`: Home Manager entry point with symlink management
- `home-manager/cli.nix`: CLI tools and terminal configurations
- `home-manager/gui.nix`: GUI applications and desktop environment
- `nixos/configuration.nix`: Base NixOS system configuration

### Current Hosts

- `lemp10`: Full NixOS system with GUI (default user: yutkat)
- `X1C10
```

</details>
