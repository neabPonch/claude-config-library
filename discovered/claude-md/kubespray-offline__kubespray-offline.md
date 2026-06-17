---
name: kubespray-offline__kubespray-offline
source: https://github.com/kubespray-offline/kubespray-offline/blob/85d52af334fd74dfddc6a41e057867f8f88860b6/CLAUDE.md
repo: kubespray-offline/kubespray-offline
kind: claude-md
stars: 113
last_pushed: 2026-05-05T12:36:33Z
license: apache-2.0
score: 9
domains: [devops, infrastructure, cli-tools]
tags: [workflow-driven, multi-stage-deployment, environment-specific]
curated: 2026-06-15
curated_by: config-scout
---

# kubespray-offline/kubespray-offline — claude-md

**Why it's worth keeping:** It excels at documenting procedural 'state changes'—showing the exact order of operations and how to validate them via CI/Docker. The inclusion of a directory structure breakdown helps the AI understand where artifacts land after multi-step scripts execute.

**Summary:** This file provides highly detailed, multi-stage workflows for two distinct environments (internet-connected vs. air-gapped). It maps specific command sequences and configuration dependencies necessary for an agent to navigate complex deployment tasks.

**Source credibility:** High; it is a practical toolset with established community interest (113 stars).

**Recency:** Very current, referencing modern OS versions and container runtimes.

**Source:** [kubespray-offline/kubespray-offline/CLAUDE.md](https://github.com/kubespray-offline/kubespray-offline/blob/85d52af334fd74dfddc6a41e057867f8f88860b6/CLAUDE.md) · 113★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Project Does

This project generates offline installation artifacts for [Kubespray](https://kubespray.io/) — a Kubernetes deployment tool. It downloads all required files (OS packages, container images, binary files, PyPI packages) on an internet-connected machine, then provides scripts to serve them locally on an air-gapped target cluster.

Supported OS: RHEL/AlmaLinux/Rocky Linux 9, Ubuntu 22.04/24.04. The current Kubespray version target is set in `target-scripts/config.sh` (`KUBESPRAY_VERSION`).

## Key Configuration

- **`target-scripts/config.sh`** — primary configuration file (Kubespray version, containerd/nerdctl/runc versions, registry port, nginx version). This file is sourced by both the download scripts (via `config.sh`) and the target node scripts.
- **`config.sh`** (root) — sources `target-scripts/config.sh` and sets the container runtime (`docker` variable, defaults to `podman`).
- **`imagelists/images.txt`** — additional container images to download beyond what Kubespray's `generate_list.sh` produces.

## Download Workflow (internet-conne
```

</details>
