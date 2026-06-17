---
name: replicatedhq__troubleshoot
source: https://github.com/replicatedhq/troubleshoot/blob/22ab3cf55192b074378c5bac82f8e1bb8fdb7dc1/CLAUDE.md
repo: replicatedhq/troubleshoot
kind: claude-md
stars: 582
last_pushed: 2026-06-11T16:15:20Z
license: apache-2.0
score: 8
domains: [cli-tools, kubernetes, infrastructure, go]
tags: [architecture-patterns, build-automation, api-evolution]
curated: 2026-06-15
curated_by: config-scout
---

# replicatedhq/troubleshoot — claude-md

**Why it's worth keeping:** The architecture section explains extension patterns (collectors/analyzers) and explicitly warns about the required 'make generate' step when modifying API types.

**Summary:** Provides essential context on Kubernetes tool workflows, specific build commands for targeted testing, and high-level architectural data flow.

**Source credibility:** High; Replicated is a reputable infrastructure company and the repo is actively maintained.

**Recency:** Current; includes context on active API version transitions.

**Source:** [replicatedhq/troubleshoot/CLAUDE.md](https://github.com/replicatedhq/troubleshoot/blob/22ab3cf55192b074378c5bac82f8e1bb8fdb7dc1/CLAUDE.md) · 582★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Replicated Troubleshoot is a Kubernetes diagnostic framework providing two kubectl plugins: `preflight` (pre-installation cluster validation) and `support-bundle` (post-installation diagnostics with log collection, redaction, and analysis). Specs use the Kubernetes custom resource format (as a serialization convention, not installed in-cluster) and are defined by application vendors and executed by cluster operators.

## Build & Test Commands

```bash
make build                        # Build bin/support-bundle and bin/preflight
make test                         # Unit tests (includes generate, fmt, vet)
make test RUN=TestMyFunction      # Run a single test
make test-integration             # Integration tests (requires k8s cluster)
make e2e                          # All e2e tests
make generate                     # Regenerate types/clients after modifying pkg/apis/
```

## Architecture

The core data flow is: **Spec loading → Collection → Redaction → Analysis → Results**. The two main workflows are orchestrated by `pkg/supportbundle/` and `pkg/
```

</details>
