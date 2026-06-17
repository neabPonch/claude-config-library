---
name: xunholy__k8s-gitops
source: https://github.com/xunholy/k8s-gitops/blob/047a3a45adaa79477493d9c4190deb7230e599c1/CLAUDE.md
repo: xunholy/k8s-gitops
kind: claude-md
stars: 634
last_pushed: 2026-06-15T00:51:26Z
license: apache-2.0
score: 9
domains: [devops, kubernetes, gitops]
tags: [fluxcd, talos, sops, taskfile]
curated: 2026-06-15
curated_by: config-scout
---

# xunholy/k8s-gitops — claude-md

**Why it's worth keeping:** Excellent directory-to-pattern mapping and specific explanation of the unique GitOps/Secret management workflows (SOPS + Flux Operator).

**Summary:** A comprehensive guide to a Kubernetes GitOps ecosystem using FluxCD and Talos Linux.

**Source credibility:** High; 600+ stars and recent activity indicate a mature, real-world infrastructure project.

**Recency:** 

**Source:** [xunholy/k8s-gitops/CLAUDE.md](https://github.com/xunholy/k8s-gitops/blob/047a3a45adaa79477493d9c4190deb7230e599c1/CLAUDE.md) · 634★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a Kubernetes GitOps repository for a personal homelab cluster managed with FluxCD and Talos Linux. The cluster follows enterprise-grade security and observability practices, showcasing CNCF ecosystem tools.

## Architecture

- **Operating System**: Talos Linux (minimal, immutable Kubernetes OS)
- **GitOps**: FluxCD with Flux Operator for declarative cluster management
- **Container Runtime**: containerd
- **Networking**: Cilium CNI with Istio service mesh
- **Storage**: Rook-Ceph, OpenEBS, democratic-csi for container-attached storage
- **Monitoring**: Prometheus, Grafana, Loki, Jaeger, Thanos for observability
- **Security**: Kyverno, OPA Gatekeeper for policy management, Falco & Tetragon for runtime security
- **Load Balancing**: MetalLB for bare metal load balancing
- **Chaos Engineering**: Litmus for chaos testing

## Directory Structure

```
├── kubernetes/                       # Kubernetes manifests and configurations
│   ├── apps/
│   │   ├── base/                     # Base application configurations (DRY principle)
│   │   │
```

</details>
