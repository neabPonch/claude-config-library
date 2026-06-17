---
name: ahembree__ansible-hms-docker
source: https://github.com/ahembree/ansible-hms-docker/blob/30e3d79c800dc0f5824843f53c3466d47b3fa158/CLAUDE.md
repo: ahembree/ansible-hms-docker
kind: claude-md
stars: 451
last_pushed: 2026-06-13T04:26:30Z
license: gpl-3.0
score: 9
domains: [devops, infrastructure-as-code, automation]
tags: [ansible, docker, deployment-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# ahembree/ansible-hms-docker — claude-md

**Why it's worth keeping:** Explains intricate internal patterns like the two-stage container map and the single-source-of-truth migration shim to prevent erroneous code generation or refactors.

**Summary:** Provides deep architectural insights into an Ansible deployment workflow, covering command workflows and complex service orchestration logic.

**Source credibility:** High; 451 stars and recent maintenance indicate a mature, popular infrastructure project.

**Recency:** 

**Source:** [ahembree/ansible-hms-docker/CLAUDE.md](https://github.com/ahembree/ansible-hms-docker/blob/30e3d79c800dc0f5824843f53c3466d47b3fa158/CLAUDE.md) · 451★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Ansible playbook that deploys a Docker-based home media server stack (Plex, Sonarr/Radarr/Prowlarr/Bazarr, Transmission + optional VPN, Traefik + Let's Encrypt, Authentik SSO, Homepage, Cloudflare DDNS, optional Tailscale/Unifi DNS) onto a single Linux host. Connection is `local` — the playbook configures the machine it runs on. Tested on Ubuntu 22.04/24.04 in CI.

## Common commands

All day-to-day workflows go through the [Makefile](Makefile):

| Command | Purpose |
|-|-|
| `make config` | Copies role defaults (`roles/hmsdocker/defaults/main/*.yml`) into `inventory/group_vars/all/` for user customization. Prompts before overwriting. |
| `make check` | Dry run with `--diff --check`. |
| `make apply` | Live apply with `--diff`. |
| `make install-reqs` | Installs galaxy roles + `community.docker` / `community.general` collections. Auto-run by `check`/`apply`. |
| `make update` | `git pull`, then rewrites deprecated variable names in `inventory/group_vars/all/*.yml` from [migrations/variable_renames.yml](migrations/variable_renames.yml), then merges ne
```

</details>
