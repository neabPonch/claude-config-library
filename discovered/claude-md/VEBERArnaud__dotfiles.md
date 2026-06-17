---
name: VEBERArnaud__dotfiles
source: https://github.com/VEBERArnaud/dotfiles/blob/f5da51f1b58cd2a7e4fc35fcca7f38dd31b92e97/CLAUDE.md
repo: VEBERArnaud/dotfiles
kind: claude-md
stars: 4
last_pushed: 2026-06-15T08:51:27Z
license: unknown
score: 9
domains: [cli-tools, devops, dotfiles, automation]
tags: [chezmoi, templates, system-config, macOS]
curated: 2026-06-15
curated_by: config-scout
---

# VEBERArnaud/dotfiles — claude-md

**Why it's worth keeping:** It provides critical 'meta-knowledge'—such as naming conventions and available Go template variables—that allows an AI to manipulate abstracted configuration files without breaking the underlying automation logic.

**Summary:** A comprehensive technical guide for managing a complex, template-driven dotfiles repository using chezmoi and Go templates.

**Source credibility:** High; the repository is actively maintained (updated months ago) and shows a highly sophisticated, professional system design.

**Recency:** Very current; explicitly references Claude Code and modern developer tools like Ghostty.

**Source:** [VEBERArnaud/dotfiles/CLAUDE.md](https://github.com/VEBERArnaud/dotfiles/blob/f5da51f1b58cd2a7e4fc35fcca7f38dd31b92e97/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a personal dotfiles repository managed by [chezmoi](https://www.chezmoi.io/) (v2.68.0+), a dotfile manager that uses Go templating to handle multiple machines with different configurations. The repository configures a complete development environment for macOS, including shell (zsh with Prezto), editor (vim with vim-plug), terminal (Ghostty), terminal multiplexer (tmux), and various development tools.

## Repository Structure

```
dotfiles/
├── .chezmoiroot              # Points to "home" as source directory
├── .chezmoiversion           # Requires chezmoi 2.68.0+
├── .github/workflows/        # CI validation (shellcheck, templates, linting)
├── .claude/                  # Project-scoped Claude Code config
│   ├── rules/chezmoi.md      # Chezmoi conventions for this repo
│   └── skills/               # Project-specific skills
│       ├── dotfiles/         # /dotfiles skill
│       └── brew-add/         # /brew-add skill
└── home/                     # Source directory for all dotfiles
    ├── .chezmoi.toml.tmpl            # Main config with featu
```

</details>
