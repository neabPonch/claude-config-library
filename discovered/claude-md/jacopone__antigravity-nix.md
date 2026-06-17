---
name: jacopone__antigravity-nix
source: https://github.com/jacopone/antigravity-nix/blob/bd2cd3d155a3efd4d85e76d18e1e99f90931bf52/CLAUDE.md
repo: jacopone/antigravity-nix
kind: claude-md
stars: 138
last_pushed: 2026-06-14T01:13:46Z
license: mit
score: 9
domains: [nix-packaging, devops, cli-tools]
tags: [nix, automation, fhs-environment, version-management]
curated: 2026-06-16
curated_by: config-scout
---

# jacopone/antigravity-nix — claude-md

**Why it's worth keeping:** Includes a specific 'Testing Checklist' to prevent breaking builds and critical instructions on converting hashes to SRI format which is a common Nix failure point.

**Summary:** Provides deep technical context for packaging proprietary binaries using Nix FHS environments and automated API-driven version updates.

**Source credibility:** High; well-maintained repo with specialized utility for the niche Nix ecosystem.

**Recency:** Current; uses modern toolsets like gh CLI and recent Nix patterns.

**Source:** [jacopone/antigravity-nix/CLAUDE.md](https://github.com/jacopone/antigravity-nix/blob/bd2cd3d155a3efd4d85e76d18e1e99f90931bf52/CLAUDE.md) · 138★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**antigravity-nix** is an auto-updating Nix Flake that packages Google Antigravity (a proprietary agentic AI platform) for NixOS and Darwin systems. It uses API endpoints to detect new versions of the Base App, IDE, and CLI tools, automatically creating PRs with updates daily at 07:00 UTC.

**Key Challenge**: The Antigravity GUI distributions are binaries that require a standard Linux filesystem layout, which conflicts with NixOS's unique structure. This is solved using `buildFHSEnv` or `autoPatchelfHook` in a multi-component architecture.

## Architecture

### Component-Based Packaging

The flake now supports three discrete packages under the `pkgs/` directory:
1. `google-antigravity` (`pkgs/google-antigravity2.nix`): The default package, for the Antigravity 2.0 Base App.
2. `google-antigravity-ide` (`pkgs/google-antigravity-ide.nix`): The Antigravity IDE.
3. `google-antigravity-cli` (`pkgs/cli.nix`): The lightweight `agy` terminal CLI.

The GUI packages share the heavy-lifting extraction and FHS-wrapping logic via `pkgs/package.nix`.

### Chrom
```

</details>
