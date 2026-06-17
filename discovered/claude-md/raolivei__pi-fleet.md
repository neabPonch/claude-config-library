---
name: raolivei__pi-fleet
source: https://github.com/raolivei/pi-fleet/blob/106a3907e260390f0d81afd06fdb47b50d2e4212/CLAUDE.md
repo: raolivei/pi-fleet
kind: claude-md
stars: 1
last_pushed: 2026-06-09T05:17:47Z
license: unknown
score: 9
domains: [infrastructure-as-code, devops, kubernetes, embedded-systems]
tags: [ansible, k3s, raspberry-pi, gitops]
curated: 2026-06-15
curated_by: config-scout
---

# raolivei/pi-fleet — claude-md

**Why it's worth keeping:** Includes 'mission-critical' procedural rules to prevent destructive AI actions (e.g., specific rsync vs dd instructions) and uses a structured 'When to Read What' index for efficient documentation navigation.

**Summary:** A highly specialized context file for managing a K3s Raspberry Pi cluster using Ansible and GitOps. It provides strict safety constraints for high-risk operations like network configuration and NVMe boot procedures.

**Source credibility:** Single star repo, but contains highly detailed, practitioner-level technical depth regarding hardware/software integration.

**Recency:** Very current; references Raspberry Pi 5 and modern FluxCD/K3s workflows.

**Source:** [raolivei/pi-fleet/CLAUDE.md](https://github.com/raolivei/pi-fleet/blob/106a3907e260390f0d81afd06fdb47b50d2e4212/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Pi Fleet - AI Assistant Context

> **Note**: This file works with Claude Code. See workspace [CLAUDE.md](../CLAUDE.md) for workspace-wide conventions and memory system details.

## Quick Reference

- **Project Type**: K3s cluster management on Raspberry Pi
- **Cluster Name**: `eldertree` (HA control plane)
- **Nodes**: `node-1`, `node-2`, `node-3` (all HA control-plane servers)
- **Control Plane VIP**: 192.168.2.100 (kube-vip)
- **Management Tools**: Ansible (system config), Terraform (infrastructure), FluxCD (GitOps)
- **Hardware**: Raspberry Pi 5 (8GB, ARM64), Debian 12 Bookworm, NVMe SSD boot

## Critical Rules

### Git Workflow
- **NEVER commit directly to main** - Always use feature branches and PRs
- **Branch prefixes**: `feat/`, `fix/`, `docs/`, `chore/`, `infra/`
- **Commit format**: `<type>: <description>` (e.g., `feat: add monitoring`, `fix: dns-config`)
- **Workflow**: `git checkout main → git pull → git checkout -b <type>/<name>`

### New LAN service (Ollie / agents)

Any new `*.eldertree.local` app **must** include in the same PR: registry entry (`docs/eldertree-local-services.yaml`), Ingress + external-dns, hosts block + `add-services-to-hosts.sh` + `Caddyfile`. Run
```

</details>
