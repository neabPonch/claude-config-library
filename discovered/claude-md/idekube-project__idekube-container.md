---
name: idekube-project__idekube-container
source: https://github.com/idekube-project/idekube-container/blob/479050da93a88ab469e687dc2a4697f1165b790a/CLAUDE.md
repo: idekube-project/idekube-container
kind: claude-md
stars: 3
last_pushed: 2026-05-28T06:58:22Z
license: mit
score: 9
domains: [devops, containerization, build-systems]
tags: [docker-bake, kubernetes, multi-arch, automation]
curated: 2026-06-15
curated_by: config-scout
---

# idekube-project/idekube-container — claude-md

**Why it's worth keeping:** The 'Self-Containment Contract' is an elite pattern; it provides a specific architectural rule followed by a command that Claude can run to audit for violations.

**Summary:** A highly sophisticated guide for a complex multi-container build system driven by Docker Bake and BuildKit named contexts. It explains the relationship between a meta-repo and its submodules/artifacts.

**Source credibility:** High-quality engineering documentation likely from a specialized research lab (SPEIT).

**Recency:** Very current, utilizing modern BuildKit/Docker Bake patterns and recent GitHub Action versions.

**Source:** [idekube-project/idekube-container/CLAUDE.md](https://github.com/idekube-project/idekube-container/blob/479050da93a88ab469e687dc2a4697f1165b790a/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

IDEKUBE is a meta-repository for IDE containers running in Kubernetes. It provides four container flavors (featured, coder, jupyter, agent) used in robotics, ML, simulation, and education at SPEIT (Shanghai Jiao Tong University).

The build system is **centralized**: a single `docker-bake.hcl` at the meta-repo root drives every image. Image submodules under `images/` are stand-alone source trees; bake supplies shared assets (artifacts, healthcheck Go source, frontend Vue source) via BuildKit named contexts so that each Dockerfile only references paths inside its own image repo.

## Repository Layout

- **`docker-bake.hcl`** — Source-of-truth bake configuration: all targets, groups, the dependency DAG (via `target:` named contexts), and per-target build args. Replaces the old `docker-builder/build.py` Python orchestrator.
- **`docker-bake.staging.hcl`** — Override file. Sets `STAGING_POSTFIX="-staging"` and `VERSION="edge"` (overridable via env). Layered after the main file with `-f`.
- **`docker-bake.production.hcl`** — Override file for producti
```

</details>
