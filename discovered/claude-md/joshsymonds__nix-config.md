---
name: joshsymonds__nix-config
source: https://github.com/joshsymonds/nix-config/blob/786dc9cfcced6c7e5684590cec15245abf5f77c6/CLAUDE.md
repo: joshsymonds/nix-config
kind: claude-md
stars: 825
last_pushed: 2026-06-12T23:16:02Z
license: mit
score: 9
domains: [infrastructure-as-code, nixos, devops, security]
tags: [nix, automation-guardrails, system-administration]
curated: 2026-06-15
curated_by: config-scout
---

# joshsymonds/nix-config — claude-md

**Why it's worth keeping:** It provides critical 'fail-fast' guardrails—like sudo pre-flighting to prevent agent hangs—and explicit warnings about high-risk procedures like secret re-keying and Git flake tracking.

**Summary:** A sophisticated operational manual for a multi-host Nix/NixOS infrastructure with deep context on secret management.

**Source credibility:** High; the repo is well-structured, active, and utilizes professional Nix/security patterns.

**Recency:** Very current; its focus on preventing agent 'hangs' and state corruption is highly relevant to modern tool-use workflows.

**Source:** [joshsymonds/nix-config/CLAUDE.md](https://github.com/joshsymonds/nix-config/blob/786dc9cfcced6c7e5684590cec15245abf5f77c6/CLAUDE.md) · 825★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# nix-config

Flake-based Nix configuration managing multiple systems.

## Systems

| Host | Platform | Description |
|------|----------|-------------|
| ninuan | macOS (aarch64-darwin) | Primary dev machine, Aerospace WM |
| ultraviolet | NixOS (x86_64-linux) | Headless server |
| bluedesert | NixOS (x86_64-linux) | Headless server |
| echelon | NixOS (x86_64-linux) | Headless server |

## Essential Commands

```bash
update                    # Rebuild current system (real binary, not an alias)
nix flake check          # Validate flake
nix build .#<package>    # Build a package
```

**IMPORTANT**: Run `update` after any Nix config changes. Nothing takes effect until rebuilt.

`update` is a `writeShellScriptBin` on `PATH` (per host: `nh os switch` for NixOS, `nh darwin switch` for macOS, ssh-into-ultraviolet for bluedesert). It works from non-interactive shells, agents, and subprocesses — no need to fall back to invoking `nh` directly. It pre-flights `sudo -n true` and refuses with a clear error if sudo would prompt, so agents fail fast instead of hanging.

**Git gotcha**: Nix flakes only see git-tracked files. Run `git add` before `nix flake check`.

## Directory Structure

```
fl
```

</details>
