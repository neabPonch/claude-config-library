---
name: vyorkin__doom
source: https://github.com/vyorkin/doom/blob/f04c3a11abf3d38de074eb920459b9790bf84d6b/CLAUDE.md
repo: vyorkin/doom
kind: claude-md
stars: 0
last_pushed: 2026-03-18T22:04:22Z
license: unlicense
score: 9
domains: [dotfiles, development-environment]
tags: [emacs, doom-emacs, configuration]
curated: 2026-06-15
curated_by: config-scout
---

# vyorkin/doom — claude-md

**Why it's worth keeping:** The use of a table to map file architecture and the explicit definition of naming conventions (the 'my/' prefix) provide perfect context for an AI agent.

**Summary:** A highly structured configuration guide for a Doom Emacs setup that maps specific files to their functional roles.

**Source credibility:** Low star count typical of personal dotfile repos, but demonstrates high-quality documentation standards.

**Recency:** Very recent, updated within the last few months.

**Source:** [vyorkin/doom/CLAUDE.md](https://github.com/vyorkin/doom/blob/f04c3a11abf3d38de074eb920459b9790bf84d6b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Doom Emacs personal configuration for Vasiliy Yorkin. Located at `~/.config/doom/` (the `$DOOMDIR`).

## Key Commands

- `doom sync` — must be run after modifying `init.el` or `packages.el` (not needed for `config.el` changes)
- `doom/reload` (`M-x doom/reload`) — reload config from within Emacs
- `doom doctor` — diagnose common issues
- `doom upgrade` — update Doom Emacs

## Architecture

The config is split across files loaded by `config.el` via Doom's `load!` macro:

| File | Purpose |
|------|---------|
| `init.el` | Doom module declarations (`doom!` block) — controls which modules are enabled |
| `packages.el` | Third-party package declarations — no `require`/`use-package!` here, just `package!` |
| `config.el` | Entry point that loads all `+*.el` files |
| `+base.el` | Fonts (JuliaMono 18), frame settings, scrolling, fringes, margins, tab-bar-notch for macOS notch |
| `+themes.el` | Theme config (base16-black-metal), italics disabled globally, custom face hooks |
| `+keys.el` | Evil keybindings — C-hjkl for window navigation, `;`/`:` swapped, l
```

</details>
