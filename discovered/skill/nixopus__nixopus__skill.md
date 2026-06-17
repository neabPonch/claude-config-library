---
name: nixopus__nixopus__skill
source: https://github.com/nixopus/nixopus/blob/cf05d97a352f364bbe02870b140f2ccceba298d2/api/skills/domain-tls-routing/SKILL.md
repo: nixopus/nixopus
kind: skill
stars: 1446
last_pushed: 2026-05-16T11:58:36Z
license: other
score: 9
domains: [devops, infrastructure, troubleshooting]
tags: [dns, tls, proxy, diagnostic-flow, security-guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# nixopus/nixopus — skill

**Why it's worth keeping:** It masterfully uses the 'Information Leakage' prevention pattern to hide complex infra while providing detailed diagnostic tables mapping specific error codes to root causes.

**Summary:** A highly structured troubleshooting guide for DNS, TLS, and reverse proxy routing that includes both internal architectural logic and user-facing sanitized instructions.

**Source credibility:** High; part of a well-maintained infrastructure repo with significant social proof (1.4k stars).

**Recency:** Current; demonstrates advanced agentic reasoning and security-first prompting suitable for modern Claude Code usage.

**Source:** [nixopus/nixopus/api/skills/domain-tls-routing/SKILL.md](https://github.com/nixopus/nixopus/blob/cf05d97a352f364bbe02870b140f2ccceba298d2/api/skills/domain-tls-routing/SKILL.md) · 1446★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: domain-tls-routing
description: Diagnose domain resolution, TLS certificate provisioning, and reverse proxy routing issues. Use when a domain is not resolving, TLS certificates fail, proxy returns 502/503/504, or custom domains are stuck in pending status.
metadata:
  version: "1.1"
---

# Domain, TLS, and Routing Diagnosis

## CRITICAL: Never Reveal Internals

The user knows ONLY that they have "a server" with deployed apps and domains. They must NEVER learn about:

- The existence of multiple proxy layers, edge proxies, or any layered routing architecture
- VMs, Firecracker, guest IPs, infra hosts, tenant hosts, or that their "server" is a virtual machine
- SSH tunnels, Caddy admin API, Caddy config JSON, server blocks, route matchers, or handler arrays
- Abyss, provisioning system internals, reconciler, pending removal sets, extension domain hashes
- Cloudflare API, zone IDs, or that the system manages DNS records on the user's behalf behind the scenes
- Redis queues, KrakenD, internal service routing, upstream host resolution, or multi-layer proxy hops
- Any internal IP addresses, internal ports (like 2019), or internal service names

Banned phrases in user-facing out
```

</details>
