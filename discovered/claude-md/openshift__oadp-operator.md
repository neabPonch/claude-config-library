---
name: openshift__oadp-operator
source: https://github.com/openshift/oadp-operator/blob/7c8f775f346704a8d53a6928dd53f597bd6d510c/CLAUDE.md
repo: openshift/oadp-operator
kind: claude-md
stars: 91
last_pushed: 2026-06-12T19:43:23Z
license: apache-2.0
score: 9
domains: [kubernetes, go, infrastructure]
tags: [operator, k8s, devops]
curated: 2026-06-15
curated_by: config-scout
---

# openshift/oadp-operator — claude-md

**Why it's worth keeping:** It includes critical 'don't-do' advice regarding branch targeting (avoiding main) and clearly defined workflows for API/manifest generation steps that prevent broken builds.

**Summary:** Provides a highly structured manual for developing a complex Kubernetes operator, including tool prerequisites, command groupings, and environment mappings.

**Source credibility:** High; part of a major OpenShift/Red Hat project with very recent updates.

**Recency:** Very current, referencing modern Go toolchains and container-native patterns.

**Source:** [openshift/oadp-operator/CLAUDE.md](https://github.com/openshift/oadp-operator/blob/7c8f775f346704a8d53a6928dd53f597bd6d510c/CLAUDE.md) · 91★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OADP (OpenShift API for Data Protection) is a Kubernetes operator that installs and manages Velero for backup and restore operations in OpenShift clusters. It extends Velero with OpenShift-specific features like Security Context Constraints (SCC), cloud credential management, and monitoring integration.

## Prerequisites

**Go Version**: Go 1.24.0 (with toolchain go1.24.5)

**macOS Users**: Install GNU sed (required for bundle generation and other targets)

```bash
brew install gnu-sed
```

**Container Tool**: Docker or Podman (auto-detected, defaults to Docker if available)

- Override with: `CONTAINER_TOOL=podman make <target>`

**Tool Version Checking**: Run `make versions` to check all tool versions and detect mismatches

## Development Commands

### Essential Commands

```bash
# Discovery and validation
make help                   # Display all available targets with descriptions
make versions               # Check tool versions and detect mismatches

# Development workflow
make test                    # Run unit tests, linting, and validati
```

</details>
