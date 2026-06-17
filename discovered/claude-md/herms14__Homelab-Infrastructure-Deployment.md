---
name: herms14__Homelab-Infrastructure-Deployment
source: https://github.com/herms14/Homelab-Infrastructure-Deployment/blob/9d51dd7aadf01ec81cf87beeb3459d3ef5d2f827/claude.md
repo: herms14/Homelab-Infrastructure-Deployment
kind: claude-md
stars: 0
last_pushed: 2026-02-16T06:33:21Z
license: unknown
score: 9
domains: [infrastructure-as-code, devops, homelab, automation]
tags: [network-topology, session-management, deployment-workflows, hybrid-cloud]
curated: 2026-06-16
curated_by: config-scout
---

# herms14/Homelab-Infrastructure-Deployment — claude-md

**Why it's worth keeping:** Demonstrates elite 'situational awareness' by mapping the entire network; implements a sophisticated multi-session protocol using session logs to prevent state drift during agent tasks.

**Summary:** An exhaustive environmental map providing IP/VLAN topology, service hierarchies, and specific deployment workflows for a hybrid Proxmox/Azure setup.

**Source credibility:** High-quality personal infrastructure documentation with clear, manual curation.

**Recency:** Highly relevant for modern agentic workflows like Claude Code that require specific environmental context and command patterns.

**Source:** [herms14/Homelab-Infrastructure-Deployment/claude.md](https://github.com/herms14/Homelab-Infrastructure-Deployment/blob/9d51dd7aadf01ec81cf87beeb3459d3ef5d2f827/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Homelab Infrastructure

IaC for Proxmox VE 9.1.2 cluster with Azure cloud integration.

## Infrastructure Summary

```
PROXMOX CLUSTER (MorpheusCluster)
├─ node01: 192.168.20.20 (TS: 100.89.33.5)  - Primary
├─ node02: 192.168.20.21 (TS: 100.96.195.27) - Services
└─ node03: 192.168.20.22 (TS: 100.88.228.34) - Hybrid Lab

NETWORKS
├─ VLAN 20: 192.168.20.0/24 - Infrastructure
├─ VLAN 40: 192.168.40.0/24 - Services
├─ VLAN 80: 192.168.80.0/24 - Hybrid Lab (AD)
└─ VLAN 90: 192.168.90.0/24 - Management

KEY HOSTS
├─ ansible:       192.168.20.30 - Ansible/Packer
├─ docker-media:  192.168.40.11 - Jellyfin, *arr
├─ docker-glance: 192.168.40.12 - Glance Dashboard
├─ docker-utils:  192.168.40.13 - Grafana, Prometheus
├─ traefik:       192.168.40.20 - Reverse Proxy
├─ authentik:     192.168.40.21 - SSO
└─ pbs:           192.168.20.50 - Proxmox Backup Server

SYNOLOGY NAS: 192.168.20.31 (DSM:5001, Plex:32400)

AZURE SUBSCRIPTIONS
├─ FireGiants-Prod: 2212d587-1bad-4013-b605-b421b1f83c30 (Primary)
├─ FireGiants-Dev:  79e34814-e81a-465c-abf3-11103880db90
└─ Nokron-Prod:     9dde5c52-88be-4608-9bee-c52d1909693f

AZURE INFRASTRUCTURE
├─ ubuntu-deploy: 10.90.10.5 - Deployment VM (Terraform/Ansible)
```

</details>
