---
name: TadMSTR__homelab-agent__claude-example
source: https://github.com/TadMSTR/homelab-agent/blob/6f87ad6c7463e7f90c5f89b787f34e5b324bcd05/claude-code/CLAUDE.md.example
repo: TadMSTR/homelab-agent
kind: claude-md
stars: 25
last_pushed: 2026-06-11T11:13:56Z
license: mit
score: 9
domains: [system-administration, agents-ai, devops]
tags: [environment-mapping, infrastructure-context, global-rules]
curated: 2026-06-15
curated_by: config-scout
---

# TadMSTR/homelab-agent — claude-md

**Why it's worth keeping:** Uses an excellent pattern of mapping absolute file paths, network dependencies (NFS/IPs), and service auth requirements that prevents repetitive prompting. The explicit distinction between global system context and project-specific context demonstrates a professional understanding of Claude Code's hierarchical loading logic.

**Summary:** A high-level system manifest designed for site-wide context in a homelab environment. It maps infrastructure, key paths, and service protocols to provide the AI with essential environmental awareness.

**Source credibility:** A specialized homelab reference with technical specificity suggesting actual usage rather than boilerplate.

**Recency:** 

**Source:** [TadMSTR/homelab-agent/claude-code/CLAUDE.md.example](https://github.com/TadMSTR/homelab-agent/blob/6f87ad6c7463e7f90c5f89b787f34e5b324bcd05/claude-code/CLAUDE.md.example) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Forge — System Context

You are operating on <your-hostname> (<hardware description>, <OS>, IP <server-ip>).
This is a dedicated AI agent server for homelab operations.

## Key Paths
- Repos: ~/repos/personal/
- Docker stacks: ~/docker/
- Docker appdata: /opt/appdata/
- Agent manifests: ~/.claude/manifests/
- Secrets: ~/.secrets/forge.env
- NATS credentials: ~/.claude-secrets/nats-agent-users.env
- Memory: ~/.claude/memory/
- Operator profile: ~/repos/gitea/agent-platform-operator/

## Infrastructure
- Operator workstation: <server-ip>
- NAS/backup: <nas-ip> — NFS: <nas-ip>:/mnt/storage/<hostname> → /mnt/nas/<hostname>
- Forge domain: <your-domain>

## Running Services
- SWAG: ports 80/443, wildcard cert <your-domain>
- Authentik: auth.<your-domain> (domain forward auth, *.<your-domain>)
- Vaultwarden: vault.<your-domain> (no forward auth — Bitwarden clients need direct access)
- Grafana: grafana.<your-domain> (OIDC via Authentik, local login disabled)
- InfluxDB: influxdb.<your-domain> (forward auth)
- SearXNG: search.<your-domain> (forward auth)
- Langfuse: langfuse.<your-domain> (forward auth)
- SigNoz: signoz.<your-domain> (forward auth)
- NATS: localhost:4222 (JetStream, per
```

</details>
