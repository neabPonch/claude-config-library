---
name: TheBeardedBearSAS__claude-craft__skill
source: https://github.com/TheBeardedBearSAS/claude-craft/blob/e9fe34b764e9ed52a8809d29cf9a471980f43b02/.claude/skills/api-gateway/SKILL.md
repo: TheBeardedBearSAS/claude-craft
kind: skill
stars: 97
last_pushed: 2026-06-14T23:39:29Z
license: mit
score: 8
domains: [backend-api, devops, infrastructure]
tags: [api-gateway, routing, traefik, kong, nginx]
curated: 2026-06-15
curated_by: config-scout
---

# TheBeardedBearSAS/claude-craft — skill

**Why it's worth keeping:** It uses specific file/keyword triggers to activate contextually relevant infra-as-code examples and includes practical YAML templates for immediate implementation.

**Summary:** Provides architectural patterns, tool comparisons, and concrete configuration snippets for API Gateway technologies like Kong and Traefik.

**Source credibility:** The repository has a respectable star count and shows very recent maintenance activity.

**Recency:** 

**Source:** [TheBeardedBearSAS/claude-craft/.claude/skills/api-gateway/SKILL.md](https://github.com/TheBeardedBearSAS/claude-craft/blob/e9fe34b764e9ed52a8809d29cf9a471980f43b02/.claude/skills/api-gateway/SKILL.md) · 97★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: api-gateway
description: API Gateway patterns (Kong, Traefik, AWS API Gateway) — rate limiting, auth, routing, versioning. Use when implementing API gateway, reverse proxy, or API management.
triggers:
  files: ["**/kong*", "**/traefik*", "**/gateway*", "**/nginx*"]
  keywords: ["api gateway", "kong", "traefik", "nginx", "rate limiting", "api management", "reverse proxy", "load balancer", "circuit breaker"]
auto_suggest: true
---

# API Gateway — Kong, Traefik, Patterns

API Gateway moderne pour routing, auth, rate limiting, observabilité.

## Responsabilités

| Fonction | Outils |
|----------|--------|
| **Routing** (path, header, canary) | Kong, Traefik, Nginx |
| **Auth** (JWT, OAuth2, API keys) | Kong plugins, Traefik middleware |
| **Rate Limiting** (per-user/IP) | Redis-backed counters |
| **Load Balancing** | HAProxy, Traefik |
| **Circuit Breaker** | Resilience4j, Istio |

## Stacks

**Kong** — Enterprise, plugins riches, K8s-native  
**Traefik** — Cloud-native, auto-discovery  
**AWS API Gateway** — Managed, serverless  
**Nginx** — Performance max, self-hosted  
**Envoy** — Service mesh (Istio), gRPC

## Kong Config

```yaml
services:
  - name: payment-api
    u
```

</details>
