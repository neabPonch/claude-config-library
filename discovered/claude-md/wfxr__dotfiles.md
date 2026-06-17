---
name: wfxr__dotfiles
source: https://github.com/wfxr/dotfiles/blob/a0417425221fd022a33e342ca393680644e59dc0/CLAUDE.md
repo: wfxr/dotfiles
kind: claude-md
stars: 100
last_pushed: 2026-03-25T15:10:26Z
license: other
score: 8
domains: [cli-tools, system-administration]
tags: [dotfiles, automation, shell, config]
curated: 2026-06-16
curated_by: config-scout
---

# wfxr/dotfiles — claude-md

**Why it's worth keeping:** It defines a specific 'Module Pattern' for adding tools and provides exact one-liner commands for syncing plugin managers (Neovim/tmux) which is highly actionable for an agent.

**Summary:** Provides structural context for a modular dotfiles repository and includes essential maintenance commands for syncing tool states.

**Source credibility:** High quality personal dotfiles with 100 stars and active maintenance.

**Recency:** 

**Source:** [wfxr/dotfiles/CLAUDE.md](https://github.com/wfxr/dotfiles/blob/a0417425221fd022a33e342ca393680644e59dc0/CLAUDE.md) · 100★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

Personal dotfiles repository managing configurations for 40+ tools across Arch Linux and macOS. Uses a modular architecture where each tool has its own directory with a `setup.sh` script.

## Commands

### Install a module
```bash
./install <module> [module...]
# Examples:
./install vim tmux
./install zsh git sdk/rust
```

### Full Arch Linux setup
```bash
./arch/setup.sh  # Requires sudo, runs multi-stage setup
```

### Sync Neovim plugins
```bash
nvim --headless "+Lazy! sync" +qa
```

### Sync tmux plugins
```bash
~/.tmux/plugins/tpm/scripts/install_plugins.sh
```

## Architecture

### Module Pattern
Each module follows this structure:
```
<module>/
├── setup.sh          # Creates symlinks to ~/.config/ or ~/
└── config files      # Tool-specific configs
```

Setup scripts use `ln -sf` / `ln -snf` to symlink configs to standard locations.

### Key Modules
- **vim/** - Neovim config using LazyVim framework (`~/.config/nvim`)
- **zsh/** - Zsh with sheldon plugin manager and starship prompt
- **tmux/** - Tmux with TPM plugin manager
- **git/**
```

</details>
