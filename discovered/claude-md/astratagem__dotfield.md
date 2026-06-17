---
name: astratagem__dotfield
source: https://github.com/astratagem/dotfield/blob/4096c6663dec845338e6fa60609c32e674e79afe/CLAUDE.md
repo: astratagem/dotfield
kind: claude-md
stars: 100
last_pushed: 2026-04-29T15:55:57Z
license: gpl-3.0
score: 9
domains: [devops, infrastructure-as-code, nixos]
tags: [nixos, dotfiles, modular]
curated: 2026-06-15
curated_by: config-scout
---

# astratagem/dotfield — claude-md

**Why it's worth keeping:** The explicit explanation of the 'Aspects System' provides the crucial mental model needed for an AI to understand cross-layer dependencies. It also defines clear command interfaces via the `just` task runner, enabling predictable system operations.

**Summary:** A modular NixOS configuration system that uses a custom 'aspects' pattern to unify NixOS and Home Manager configurations across multiple hosts.

**Source credibility:** Highly credible with 100 stars and recent maintenance history.

**Recency:** Current; uses modern Nix Flake and Colmena workflows.

**Source:** [astratagem/dotfield/CLAUDE.md](https://github.com/astratagem/dotfield/blob/4096c6663dec845338e6fa60609c32e674e79afe/CLAUDE.md) · 100★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Dotfield - NixOS Configuration

## Overview

Dotfield is a comprehensive NixOS configuration system ("dotfiles") using Nix
flakes for managing multiple machines and users. It's built around a modular
architecture with features, hosts, and users as the primary organizational
units.

## Project Structure

```text
/etc/nixos/
├── flake.nix              # Main flake definition with inputs and outputs
├── hive.nix               # Colmena deployment configuration
├── src/                   # Main source code
│   ├── features/          # Modular feature configurations
│   ├── hosts/             # Host-specific configurations
│   ├── lib/               # Custom Nix library functions
│   ├── meta/              # Metadata and constants
│   ├── modules/           # Custom NixOS/Home Manager modules
│   ├── packages/          # Custom package definitions
│   └── users/             # User-specific configurations
├── dev/                   # Development environment tools
├── tests/                 # Test configurations
├── secrets/               # SOPS-encrypted secrets
├── overlays/              # Nix package overlays
└── npins/                 # Pinned dependencies
```

## Key Technologies &
```

</details>
