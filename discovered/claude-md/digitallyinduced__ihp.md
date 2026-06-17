---
name: digitallyinduced__ihp
source: https://github.com/digitallyinduced/ihp/blob/5f02814d472a496318dfef994cbefeeb489de78a/CLAUDE.md
repo: digitallyinduced/ihp
kind: claude-md
stars: 5291
last_pushed: 2026-06-14T15:17:34Z
license: mit
score: 9
domains: [backend-api, web-framework, haskell]
tags: [monorepo, hasql, nix, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# digitallyinduced/ihp — claude-md

**Why it's worth keeping:** The 'echo | ghci' pattern solves the stdin-blocking issue in Haskell development, and the detailed Hasql layering example provides a perfect architectural template for type-safe database interaction.

**Summary:** Provides comprehensive environment setup and architectural guidance for a complex Haskell monorepo. It includes specific workflows for fast iterative testing using GHCi to bypass slow Nix builds.

**Source credibility:** Extremely high; sourced from a major, highly-starred, and actively maintained web framework.

**Recency:** 

**Source:** [digitallyinduced/ihp/CLAUDE.md](https://github.com/digitallyinduced/ihp/blob/5f02814d472a496318dfef994cbefeeb489de78a/CLAUDE.md) · 5291★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

IHP (Integrated Haskell Platform) is a batteries-included Haskell web framework built on Haskell and Nix. It follows an MVC architecture with type-safe routing, HSX templating (JSX-like syntax for HTML), and PostgreSQL as the database.

## Development Environment Setup

IHP uses devenv.sh (a wrapper around `nix develop` and `direnv`) for development:

```bash
cd /path/to/ihp
direnv allow
```

Alternatively, use `nix develop` directly to enter a dev shell. You can also use `direnv exec .` to get a cached nix develop environment.

## Running Tests

Prefer `ghci` for quick type checking and iteration — full nix builds (`nix flake check`) are slow. Use ghci interactively or via `echo ... | ghci` one-liners for fast feedback.

**When using ghci, keep in mind that it expects input on stdin. If you don't provide any, ghci will never return.** The `echo ... | ghci` pattern handles this correctly by piping input.

**IHP IDE Tests** (from the repo root):
```bash
# Interactive (allows :r to reload after changes):
ghci
:l ihp-ide/Test/Main.hs
main
:r
main

# One-lin
```

</details>
