---
name: ryanseipp__homelab
source: https://github.com/ryanseipp/homelab/blob/9d6ac1c5ee62987bea4c611a941b78986679b8bb/CLAUDE.md
repo: ryanseipp/homelab
kind: claude-md
stars: 3
last_pushed: 2025-11-12T02:30:44Z
license: mit
score: 9
domains: [devops, kubernetes, infrastructure-as-code]
tags: [gitops, talos, nixos, k8s]
curated: 2026-06-16
curated_by: config-scout
---

# ryanseipp/homelab — claude-md

**Why it's worth keeping:** Contains highly transferable 'Service Lifecycle' recipes (adding/updating services) and strict warnings against manual edits of generated artifacts. The inclusion of specific CLI command patterns for specialized tools like talosctl and rook-ceph is excellent.

**Summary:** Provides comprehensive guidance for a complex GitOps-driven homelab using Talos Linux and ArgoCD. It bridges high-level architecture with granular operational procedures.

**Source credibility:** High; written by an experienced engineer managing a sophisticated bare-metal infrastructure.

**Recency:** 

**Source:** [ryanseipp/homelab/CLAUDE.md](https://github.com/ryanseipp/homelab/blob/9d6ac1c5ee62987bea4c611a941b78986679b8bb/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Overview

This is a declarative homelab configuration combining NixOS host management with
Kubernetes cluster management. The repository uses Talos Linux for Kubernetes
cluster provisioning and ArgoCD for GitOps-based application deployment.

## Architecture

### Two-Layer Infrastructure

1. **NixOS Host Layer** (deprecated/transitioning):
   - `flake.nix`: Defines NixOS system configurations using flake-parts
   - Previously configured bare-metal Kubernetes with Cilium CNI
   - Deploy mechanism: `deploy-rs` for remote NixOS deployments
   - Host configuration references in flake.nix point to now-deleted
     `nix/hosts/kube-host-1`

2. **Kubernetes Cluster Layer** (current):
   - **Talos Linux**: Kubernetes cluster OS (configs in `clusters/home/talos/`)
   - **GitOps**: ArgoCD ApplicationSets manage all cluster applications
   - **Manifest Management**: Helm charts templated to static YAML, managed via
     Kustomize

### Cluster Configuration Pattern

Each service in `clusters/home/` follows this structure:

- `helmfile.yaml`: Helm chart definitions with values
```

</details>
