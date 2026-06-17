---
name: kube-logging__logging-operator
source: https://github.com/kube-logging/logging-operator/blob/a26b7d60df04af01781064c9eab574b92cccca50/CLAUDE.md
repo: kube-logging/logging-operator
kind: claude-md
stars: 1695
last_pushed: 2026-06-15T15:24:39Z
license: apache-2.0
score: 9
domains: [kubernetes, go, infrastructure, devops]
tags: [operator, k8s, golang, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# kube-logging/logging-operator — claude-md

**Why it's worth keeping:** Uses 'Key Patterns' to explain intent (Repository Pattern, Reconciler Chain) and provides critical module-specific navigation instructions to prevent import errors.

**Summary:** Provides deep architectural context for a complex Kubernetes operator including multi-module Go navigation and design patterns.

**Source credibility:** High; highly starred, actively maintained production-grade Kubernetes operator.

**Recency:** Current; follows modern Go multi-module patterns relevant to today's development workflows.

**Source:** [kube-logging/logging-operator/CLAUDE.md](https://github.com/kube-logging/logging-operator/blob/a26b7d60df04af01781064c9eab574b92cccca50/CLAUDE.md) · 1695★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Kubernetes operator that manages a complete logging pipeline. It deploys and configures:
- **Fluent Bit** (DaemonSet) — collects logs from every node
- **Fluentd or syslog-ng** (StatefulSet) — aggregates and routes logs to outputs

Users define `Flow`/`Output` CRDs (or their cluster-scoped equivalents) to route logs to destinations like S3, Elasticsearch, Loki, Kafka, etc.

## Project Structure

```
logging-operator/
├── .github/                         # GitHub Actions workflows
├── charts/logging-operator/         # Helm chart (synced with manifests via make manifests)
├── controllers/
│   ├── logging/                     # Core reconcilers (Logging, LoggingRoute, TelemetryController, AxoSyslog)
│   └── extensions/                  # EventTailer and HostTailer reconcilers
├── e2e/                             # KIND-based e2e test suites
├── images/
│   ├── config-reloader/             # Sidecar that hot-reloads on ConfigMap/Secret change
│   ├── fluentd/                     # Custom Fluentd Docker image (Ruby gems, fluent.conf)
│   ├─
```

</details>
