---
name: pulumi__pulumi-kubernetes-operator
source: https://github.com/pulumi/pulumi-kubernetes-operator/blob/058cbd8c12f8165c79abf89385553380d6cbfbc1/CLAUDE.md
repo: pulumi/pulumi-kubernetes-operator
kind: claude-md
stars: 288
last_pushed: 2026-06-13T08:39:05Z
license: apache-2.0
score: 9
domains: [kubernetes-operator, infrastructure-as-code, go]
tags: [architecture-heavy, workflow-automation, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# pulumi/pulumi-kubernetes-operator — claude-md

**Why it's worth keeping:** The 'Important Patterns' section is exceptional, explaining architectural intent (finalizers, field indexing) that code alone doesn't reveal. It also explicitly maps out complex, multi-file release procedures.

**Summary:** Provides a deep architectural mental model of the operator-agent relationship and includes structured command sets for multi-directory builds.

**Source credibility:** High; maintained by Pulumi, an industry leader in infrastructure-as-code.

**Recency:** Very current; reflects modern Go and Kubernetes development patterns.

**Source:** [pulumi/pulumi-kubernetes-operator/CLAUDE.md](https://github.com/pulumi/pulumi-kubernetes-operator/blob/058cbd8c12f8165c79abf89385553380d6cbfbc1/CLAUDE.md) · 288★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

The Pulumi Kubernetes Operator is a Kubernetes operator that provides a CI/CD workflow for Pulumi stacks using Kubernetes primitives. It allows users to adopt a GitOps workflow for managing cloud infrastructure by creating Stack resources as first-class Kubernetes API resources.

## Architecture

The project consists of two main executable components:

### Operator Manager (`operator/`)
- The main control plane component running in the cluster
- Uses Kubernetes controller-runtime framework
- Implements 4 primary controllers:
  - **StackReconciler** - Manages Stack CRs (pulumi.com/v1 and v1alpha1)
  - **WorkspaceReconciler** - Manages Workspace CRs (auto.pulumi.com/v1alpha1)
  - **UpdateReconciler** - Manages Update CRs (auto.pulumi.com/v1alpha1)
  - **ProgramReconciler** - Manages Program CRs (pulumi.com/v1)

### Agent (`agent/`)
- A gRPC service running inside workspace pods
- Executes actual Pulumi operations (up, destroy, preview, refresh)
- Uses Pulumi Automation API to interact with Pulumi stacks
- Communicates with the operator via gRPC wit
```

</details>
