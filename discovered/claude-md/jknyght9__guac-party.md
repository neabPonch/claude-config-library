---
name: jknyght9__guac-party
source: https://github.com/jknyght9/guac-party/blob/eb3bc1279affd276f4b6a448e82b6b2325a88cdb/CLAUDE.md
repo: jknyght9/guac-party
kind: claude-md
stars: 2
last_pushed: 2026-04-15T01:02:10Z
license: unknown
score: 9
domains: [devops, infrastructure-as-code, cli-tools]
tags: [hashicorp, terraform, nomad, automation]
curated: 2026-06-15
curated_by: config-scout
---

# jknyght9/guac-party — claude-md

**Why it's worth keeping:** It provides explicit service discovery/routing patterns, detail on exact command execution through Docker wrappers, and clear sequences of manual intervention steps.

**Summary:** A highly technical guide for a complex infrastructure deployment pipeline using Proxmox, Terraform, and HashiCorp Nomad.

**Source credibility:** Small-scale personal project but demonstrates high-level DevOps expertise.

**Recency:** Very recent (2 months ago) and highly relevant to current tool versions.

**Source:** [jknyght9/guac-party/CLAUDE.md](https://github.com/jknyght9/guac-party/blob/eb3bc1279affd276f4b6a448e82b6b2325a88cdb/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Guac-Party deploys HA Apache Guacamole on a Proxmox cluster via HashiCorp Nomad. The admin workstation only needs Docker — Packer, Terraform, and Nomad CLI all run in containers via wrapper scripts in `docker/`.

## Pipeline

The deployment is a linear pipeline with manual steps between stages:

1. **`bootstrap/bootstrap.sh`** — Interactive. Creates Proxmox automation user/role/token, SDN, SSH keys, generates `terraform.tfvars` and `.env`, then invokes Packer and Terraform.
2. **Packer** (`docker/packer.sh`) — Builds Ubuntu 24.04 VM template with Docker CE + Nomad pre-installed.
3. **Terraform** (`docker/terraform.sh`) — Clones one Nomad VM per Proxmox node. Cloud-init writes Nomad config and starts the cluster.
4. **`nomad/deploy.sh`** — Deploys jobs in order: Vault → Traefik → Authentik → Guacamole. Pauses for manual Vault init/unseal and Authentik OIDC setup.

## Key Commands

```bash
# Full bootstrap (interactive, runs everything)
./bootstrap/bootstrap.sh

# Docker-wrapped tool invocations
./docker/terraform.sh init
./docker/terraform.sh appl
```

</details>
