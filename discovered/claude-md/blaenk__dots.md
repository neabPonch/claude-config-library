---
name: blaenk__dots
source: https://github.com/blaenk/dots/blob/43c5aa7a0de434baa457f5cc552c4277258084ec/CLAUDE.md
repo: blaenk/dots
kind: claude-md
stars: 56
last_pushed: 2026-06-15T13:36:51Z
license: unknown
score: 9
domains: [cli-tools, dotfiles, shell]
tags: [chezmoi, tmux, zsh, automation]
curated: 2026-06-15
curated_by: config-scout
---

# blaenk/dots — claude-md

**Why it's worth keeping:** It includes specific deployment workflows (chezmoi apply) and provides high-value syntax guardrails for tmux that prevent common LLM configuration errors.

**Summary:** Provides a comprehensive map of how source templates in this repository are deployed to the system via chezmoi.

**Source credibility:** A legitimate personal dotfiles repository with active maintenance and decent star count.

**Recency:** Highly current, specifically mentioning Claude Code integration.

**Source:** [blaenk/dots/CLAUDE.md](https://github.com/blaenk/dots/blob/43c5aa7a0de434baa457f5cc552c4277258084ec/CLAUDE.md) · 56★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A chezmoi-managed dotfiles repository. Files here are source templates/configs that chezmoi deploys to `~`. The working directory is `~/.local/share/chezmoi`.

## Chezmoi Conventions

- `dot_` prefix → `.` in target (e.g., `dot_tmux.conf` → `~/.tmux.conf`)
- `dot_config/` → `~/.config/`
- `private_` prefix → deployed with restricted permissions (e.g., `private_atuin`, `private_fish`)
- `executable_` prefix → deployed with execute bit set
- `.tmpl` suffix → Go template, rendered by chezmoi before deployment
- `.chezmoiignore` lists files tracked in git but NOT deployed (e.g., `Brewfile`, `readme.md`, `zsh/`, `iterm2/`)
- Apply changes: `chezmoi apply` (or `chezmoi apply ~/.tmux.conf` for a single file)
- Preview diff: `chezmoi diff`
- Edit source from target path: `chezmoi edit ~/.tmux.conf`

## Key Config Files

| Source | Target | Notes |
|--------|--------|-------|
| `dot_tmux.conf` | `~/.tmux.conf` | Extensive tmux config, vi-mode, 3-line status bar |
| `dot_zshrc` | `~/.zshrc` | Zinit plugin manager, lazy-loaded plugins |
| `dot_zshenv` | `~/.zsh
```

</details>
