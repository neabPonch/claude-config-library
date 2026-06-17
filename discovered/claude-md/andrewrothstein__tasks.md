---
name: andrewrothstein__tasks
source: https://github.com/andrewrothstein/tasks/blob/89a4008272b7163e53adf5dd4c54765d3e542b3e/CLAUDE.md
repo: andrewrothstein/tasks
kind: claude-md
stars: 2
last_pushed: 2026-05-16T23:21:28Z
license: mit
score: 9
domains: [devops, kubernetes, infrastructure]
tags: [taskfile, k8s, automation]
curated: 2026-06-16
curated_by: config-scout
---

# andrewrothstein/tasks — claude-md

**Why it's worth keeping:** It provides highly specific command patterns including environment variable usage and offers decision logic for selecting different CNI/cluster configurations.

**Summary:** An operational guide for a DevOps toolkit using Taskfile to manage Kubernetes cluster lifecycles and application deployments.

**Source credibility:** High-quality, structured documentation typical of professional infrastructure automation repositories.

**Recency:** Current, utilizing modern tools like Talos, K3d, and Taskfile.

**Source:** [andrewrothstein/tasks/CLAUDE.md](https://github.com/andrewrothstein/tasks/blob/89a4008272b7163e53adf5dd4c54765d3e542b3e/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a DevOps/Infrastructure automation toolkit using [Taskfile](https://taskfile.dev/) as the primary build system. The repository contains three main categories of task definitions:

1. **Cluster Lifecycle Management**: Tasks for creating and managing ephemeral Kubernetes clusters (Kind, K3d, Talos)
2. **Application Deployment**: Tasks for deploying applications, operators, and services into any Kubernetes cluster
3. **External Cluster Support**: BYO (Bring Your Own) cluster integration for production environments (Harvester, EKS, GKE, etc.)

## Repository Organization

### Cluster Lifecycle Management (Ephemeral Clusters)
These tasks handle provisioning and teardown of local development clusters:

**Core Cluster Provisioning:**
- `kind.yml` - Basic Kind cluster setup
- `k3d.yml` - K3d cluster with extensive configuration options
- `talos.yml` - Talos Linux Kubernetes clusters
- `byo-cluster.yml` - External cluster support (no-op create/delete)

**Kind with CNI Variants:**
- `kind+antrea.yml` - Kind cluster with Antrea CNI
- `kind+calico.yml` - Kind
```

</details>
