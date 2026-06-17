---
name: zngtfy__zngtfy__csnp-infra-claude
source: https://github.com/zngtfy/zngtfy/blob/f8fa593e8821403e3e06d7f737c5e066c7ddf7bd/CLAUDE/csnp-infra-CLAUDE.md
repo: zngtfy/zngtfy
kind: claude-md
stars: 0
last_pushed: 2026-05-24T05:27:00Z
license: unknown
score: 9
domains: [devops, infrastructure-as-code]
tags: [terraform, ansible, proxmox, inventory]
curated: 2026-06-16
curated_by: config-scout
---

# zngtfy/zngtfy — claude-md

**Why it's worth keeping:** The inclusion of a highly detailed VM inventory table (VMIDs, IPs, specs) gives Claude immediate ground truth for networking/provisioning tasks; it also clearly defines the 'authoritative' source hierarchy.

**Summary:** Provides a comprehensive technical map of an IaC environment involving Terraform, Ansible, and Proxmox.

**Source credibility:** Low social proof (0 stars), but the content demonstrates high-density, professional-grade infrastructure mapping.

**Recency:** Highly current, referencing modern stacks like Ubuntu 24.04 and specific Terraform/Ansible workflows.

**Source:** [zngtfy/zngtfy/CLAUDE/csnp-infra-CLAUDE.md](https://github.com/zngtfy/zngtfy/blob/f8fa593e8821403e3e06d7f737c5e066c7ddf7bd/CLAUDE/csnp-infra-CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CSNP Infra — Codebase Guide for Claude

## Project Overview

**`csnp-infra`** is the **Infrastructure-as-Code and runtime configuration repository** for the entire CSNP ecosystem. This repo contains Terraform (VM provisioning), Ansible (configuration management), Nginx edge proxy configs, and Kubernetes setup scripts.

**Scope:** This repo is the **execution layer** — implements the procedures defined in `csnp-docs`. If there is a conflict, `csnp-docs` is authoritative.

**Current environment:** DEV only. UAT/PRO requires architecture review + security approval + state backend hardening before promoting.

**Architecture documentation:** https://github.com/skg-csnp/csnp-docs

---

## Repository Structure

```
csnp-infra/
├── platforms/
│   ├── aws/                     # AWS infrastructure (future)
│   │   ├── kubernetes/
│   │   └── terraform/
│   └── proxmox/                 # Proxmox VE platform
│       ├── terraform/           # VM provisioning (Proxmox VE, post-clone only)
│       │   ├── envs/
│       │   │   ├── dev/         # DEV environment — VM definitions per service
│       │   │   │   ├── backend.tf       # Local state backend
│       │   │   │   ├── variables.tf     #
```

</details>
