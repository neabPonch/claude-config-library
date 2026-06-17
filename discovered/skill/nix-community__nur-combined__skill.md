---
name: nix-community__nur-combined__skill
source: https://github.com/nix-community/nur-combined/blob/38797c907608bed842233e3083c9fd66a2a46cde/repos/lmdevv/.agents/skills/nix/SKILL.md
repo: nix-community/nur-combined
kind: skill
stars: 192
last_pushed: 2026-06-15T08:23:43Z
license: unknown
score: 8
domains: [cli-tools, devops]
tags: [nix, package-management, environment]
curated: 2026-06-15
curated_by: config-scout
---

# nix-community/nur-combined — skill

**Why it's worth keeping:** It highlights specific non-interactive workflows like `nix eval` and shebang-based execution which are critical for agentic tool use in headless environments.

**Summary:** Provides actionable patterns for using Nix to manage transient dependencies and evaluate expressions without a REPL.

**Source credibility:** High-quality technical documentation curated by the Nix community.

**Recency:** 

**Source:** [nix-community/nur-combined/repos/lmdevv/.agents/skills/nix/SKILL.md](https://github.com/nix-community/nur-combined/blob/38797c907608bed842233e3083c9fd66a2a46cde/repos/lmdevv/.agents/skills/nix/SKILL.md) · 192★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nix
description: Run packages temporarily, create isolated shell environments, and evaluate Nix expressions. Use when executing tools without installing, debugging derivations, or searching nixpkgs.
---

# Nix Skill

Nix is a powerful package manager and functional programming language. This skill covers common operations like running apps on-the-fly and managing environments.

## Running Applications

You can run any application from `nixpkgs` without installing it permanently.

```bash
# Run a package once
nix run nixpkgs#hello

# Run a package with specific arguments
nix run nixpkgs#cowsay -- "Hello from Nix!"

# Run a command within a shell environment (non-interactive)
nix shell nixpkgs#git nixpkgs#vim --command git --version

# Run long-running applications (e.g., servers): `tmux new -d 'nix run nixpkgs#some-server'`
```

## Formatting

Format Nix files in your project:

```bash
# Format current flake
nix fmt

# Check formatting
nix fmt -- --check
```

## Evaluating Expressions (Debugging)

Since the environment is headless and non-interactive, use `nix eval` instead of the REPL for debugging.

```bash
# Evaluate a simple expression
nix eval --expr '1 + 2'

# Inspec
```

</details>
