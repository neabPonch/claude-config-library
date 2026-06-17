---
name: Project-HAMi__HAMi
source: https://github.com/Project-HAMi/HAMi/blob/df6ac09e0420fd337133eb673d7fe72269dd194e/CLAUDE.md
repo: Project-HAMi/HAMi
kind: claude-md
stars: 3567
last_pushed: 2026-06-15T03:38:57Z
license: apache-2.0
score: 9
domains: [infrastructure, kubernetes, systems-programming]
tags: [architecture, go, k8s, build-commands]
curated: 2026-06-15
curated_by: config-scout
---

# Project-HAMi/HAMi — claude-md

**Why it's worth keeping:** It teaches the AI how to extend functionality via a clear 'Device Registration Pattern' and enforces strict coding conventions like K8s import aliases.

**Summary:** Provides deep architectural context, component interactions, and specific patterns for hardware backend registration.

**Source credibility:** High; high-star CNCF sandbox project with very recent activity.

**Recency:** Extremely current, featuring specific tool versions and modern Go development workflows.

**Source:** [Project-HAMi/HAMi/CLAUDE.md](https://github.com/Project-HAMi/HAMi/blob/df6ac09e0420fd337133eb673d7fe72269dd194e/CLAUDE.md) · 3567★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

HAMi (Heterogeneous AI Computing Virtualization Middleware) is a CNCF sandbox project that provides device virtualization for heterogeneous AI accelerators (GPU, NPU, DCU, etc.) in Kubernetes. It enables device sharing, memory/core isolation, and topology-aware scheduling across multiple hardware vendors.

## Build Commands

```bash
make build              # Build all binaries (scheduler, vGPUmonitor, nvidia-device-plugin) to bin/
make docker             # Build Docker image
make tidy               # Run go mod tidy
make test               # Run unit tests with coverage (output in _output/coverage/)
make lint               # Run golangci-lint v2.8.0 (via hack/verify-staticcheck.sh)
make verify             # Run all verification checks (license, lint, import aliases)
```

### Running a single test

```bash
go test ./pkg/scheduler/... -run TestSpecificFunc -short --race -count=1
go test ./pkg/device/nvidia/... -run TestName -short --race -count=1
```

### Binary targets (from version.mk)

- `scheduler` — the scheduler extender
- `vGPUmonitor` — in-
```

</details>
