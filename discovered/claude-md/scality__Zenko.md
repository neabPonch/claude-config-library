---
name: scality__Zenko
source: https://github.com/scality/Zenko/blob/835a6459803d1a716337a43ce28587e3d4c381c3/CLAUDE.md
repo: scality/Zenko
kind: claude-md
stars: 669
last_pushed: 2026-06-15T18:44:50Z
license: apache-2.0
score: 8
domains: [infrastructure, cloud-native, devops]
tags: [toolchain-mapping, multi-runtime]
curated: 2026-06-16
curated_by: config-scout
---

# scality/Zenko — claude-md

**Why it's worth keeping:** It prevents environment mismatch by detailing exact Node/Python/JRE versions required for different task contexts (e.g., Node 22 vs 24).

**Summary:** Maps complex multi-component architecture to specific directories and defines explicit runtime versions across various subprojects.

**Source credibility:** High; Scality is an established enterprise entity with high-frequency repository maintenance.

**Recency:** Very current; uses modern runtimes like Node 24 and mentions AI agent integration workflows.

**Source:** [scality/Zenko/CLAUDE.md](https://github.com/scality/Zenko/blob/835a6459803d1a716337a43ce28587e3d4c381c3/CLAUDE.md) · 669★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Zenko

**Scality's open-source multi-cloud data controller** — a Kubernetes-based deployment of the Zenko stack. The actual service implementations (cloudserver, backbeat, vault2, sorbet, scuba, s3utils, pensieve-api, kafka-cleaner, drctl, zenko-operator) live in separate repos; this repo packages, versions, integration-tests, and releases them together.

## What lives here

- `solution/deps.yaml`, `solution-base/deps.yaml` — image/registry/tag manifests for every Zenko component
- `solution/zenkoversion.yaml` — `ZenkoVersion` CR template (dashboards, policies, feature flags, capabilities, location types)
- `solution/kafka/Dockerfile`, `solution/kafka-connect/Dockerfile` — Scality-built Kafka + Kafka Connect images
- `solution-base/mongodb/` — MongoDB Helm charts and patches
- `tests/functional/ctst/` — TypeScript Cucumber end-to-end tests
- `tests/workflows/` — TypeScript Jest tests for CI tooling
- `tests/zenko_tests/` — Python + Node.js integration tests
- `monitoring/` — Prometheus rules, Grafana dashboards
- `.github/workflows/` — CI pipelines (`end2end`, `release`, `review`, `alerts`)

## Toolchains

Multiple runtimes in play — check the specific subproject's Dockerfile / w
```

</details>
