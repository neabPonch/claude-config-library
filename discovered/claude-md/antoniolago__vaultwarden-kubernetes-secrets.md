---
name: antoniolago__vaultwarden-kubernetes-secrets
source: https://github.com/antoniolago/vaultwarden-kubernetes-secrets/blob/0b26108b2f015047633ee54381380e5f4505ded9/CLAUDE.md
repo: antoniolago/vaultwarden-kubernetes-secrets
kind: claude-md
stars: 83
last_pushed: 2026-05-27T13:01:50Z
license: mit
score: 9
domains: [backend, web-frontend, devops, security]
tags: [.net, react, kubernetes, helm]
curated: 2026-06-15
curated_by: config-scout
---

# antoniolago/vaultwarden-kubernetes-secrets — claude-md

**Why it's worth keeping:** Includes 'Important Implementation Details' to prevent logic errors and 'Common Development Workflows' to guide complex cross-component changes.

**Summary:** A comprehensive guide covering multi-component architecture (C# backend, React frontend, Helm charts) and specific domain logic constraints.

**Source credibility:** High; a well-maintained repository with significant stars and recent updates.

**Recency:** Very current, referencing modern technologies like .NET 10.0 and Bun.

**Source:** [antoniolago/vaultwarden-kubernetes-secrets/CLAUDE.md](https://github.com/antoniolago/vaultwarden-kubernetes-secrets/blob/0b26108b2f015047633ee54381380e5f4505ded9/CLAUDE.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Vaultwarden Kubernetes Secrets is a service that automatically synchronizes secrets from Vaultwarden (a Bitwarden-compatible server) to Kubernetes Secrets. It consists of four main components:

1. **VaultwardenK8sSync** - Main sync service (console app)
2. **VaultwardenK8sSync.Api** - REST API for monitoring and control
3. **VaultwardenK8sSync.Database** - SQLite database for state tracking
4. **dashboard** - React/TypeScript frontend for monitoring

## Architecture

### C# Projects (.NET 10.0)

The main sync service follows a layered architecture:

- **Application/** - Application host and command handlers
- **Infrastructure/** - Cross-cutting concerns (ProcessLock, ProcessRunner, MetricsServer, GlobalSyncLock)
- **Services/** - Core business logic (SyncService, VaultwardenService, KubernetesService, WebhookService, MetricsService)
- **Models/** - Domain entities (VaultwardenItem, WebhookEvent, SyncSummary)
- **Configuration/** - Settings and constants
- **HealthChecks/** - Health check implementations
- **Policies/** - Resilience policies (Poll
```

</details>
