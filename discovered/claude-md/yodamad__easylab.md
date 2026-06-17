---
name: yodamad__easylab
source: https://github.com/yodamad/easylab/blob/4a1120037370ca7ea137e180708651fc0ede7b74/CLAUDE.md
repo: yodamad/easylab
kind: claude-md
stars: 9
last_pushed: 2026-06-12T14:11:31Z
license: mit
score: 8
domains: [backend, infrastructure-as-code, go]
tags: [guardrails, architecture-mapping, devops]
curated: 2026-06-16
curated_by: config-scout
---

# yodamad/easylab — claude-md

**Why it's worth keeping:** The 'Must NOT' section is an elite technique for controlling agent behavior; the detailed file tree includes functional descriptions that build a mental model of how data flows through the system.

**Summary:** Provides deep architectural context and strict behavioral guardrails to prevent AI-driven code drift in a complex infrastructure project.

**Source credibility:** Low star count, but the highly structured and professional documentation suggests a high-quality project.

**Recency:** Very current, referencing modern tech stacks like Go 1.26 and HTMX.

**Source:** [yodamad/easylab/CLAUDE.md](https://github.com/yodamad/easylab/blob/4a1120037370ca7ea137e180708651fc0ede7b74/CLAUDE.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# EasyLab — Claude Code Rules

## Project Overview

EasyLab is a Go web application that provisions cloud-based lab environments using Pulumi IaC on OVHcloud. It deploys Kubernetes clusters with Coder workspaces for workshop participants.

Two main entry points:
1. A Pulumi program (`main.go`) for infrastructure provisioning
2. A web server (`cmd/server/main.go`) with an HTMX-powered admin/student UI

### Tech Stack

- Go 1.26 with `html/template` for server-side rendering
- HTMX for dynamic UI interactions (no frontend framework)
- Pulumi SDK v3 for infrastructure as code (Go-based programs)
- OVHcloud provider for cloud resources (network, k8s, node pools)
- Coder SDK for workspace and template management
- `net/http` with `http.ServeMux` for routing (no external router)
- Playwright for E2E frontend testing
- Makefile for build, test, and CI tasks
- Docker + docker-compose for containerized deployment
- Kustomize manifests for Kubernetes deployment (`k8s-deployment/`)
- MkDocs for documentation (`docs/`)

### Folder Structure

```
main.go                  # Pulumi IaC entry point (OVH infra + k8s + Coder setup)
cmd/
  server/
    main.go              # Web server entry point (HT
```

</details>
