---
name: babeal__dotfiles__plan-skill
source: https://github.com/babeal/dotfiles/blob/b8b0395b2135f30ab5860b6aed3d9d77dd833805/docs/bak/plan-skill.md
repo: babeal/dotfiles
kind: skill
stars: 1
last_pushed: 2026-04-10T19:38:43Z
license: unknown
score: 8
domains: [devops, cli-tools, automation]
tags: [infrastructure-as-code, environment-setup, dynamic-testing]
curated: 2026-06-15
curated_by: config-scout
---

# babeal/dotfiles — skill

**Why it's worth keeping:** Provides a concrete pattern for injecting state via TOML files and replacing absolute paths/usernames with dynamic build arguments and shell variables to prevent execution failure across different hosts.

**Summary:** A technical redesign focused on transforming hardcoded environment tests into dynamic, portable agent skills using Docker and externalized configuration.

**Source credibility:** Personal dotfiles repo; low popularity but shows professional-grade infrastructure logic.

**Recency:** Very recent, updated 2 months ago.

**Source:** [babeal/dotfiles/docs/bak/plan-skill.md](https://github.com/babeal/dotfiles/blob/b8b0395b2135f30ab5860b6aed3d9d77dd833805/docs/bak/plan-skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill & Testing Infrastructure Redesign

**Design reference:** [docs/design/testing.md](design/testing.md)

This plan closes the gap between the current state and the design: dynamic username, correct UID, multiple named test configs, externalized environment config, and updated skills.

---

## Current State

- `Dockerfile.ubuntu` — hardcoded `babeal`, no build args
- `docker-compose.yml` — no USERNAME build arg passthrough
- `tests/e2e/config/chezmoi.toml` — single config, `install_packages=true`
- `test-ubuntu-docker` SKILL.md — hardcoded `babeal` and absolute host paths
- `test-macos` SKILL.md — needs environment config reference

---

## Phase 1: Rename and Fix the Dockerfile

### 1a. Rename

```bash
git mv tests/e2e/ubuntu/Dockerfile.ubuntu tests/e2e/ubuntu/Dockerfile
```

### 1b. Replace contents

```dockerfile
FROM ubuntu:24.04

ARG USERNAME=brandt
ARG USER_UID=1001
ARG USER_GID=$USER_UID

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y --no-install-recommends \
    curl git sudo zsh rsync locales build-essential ca-certificates \
    && locale-gen en_US.UTF-8 \
    && rm -rf /var/lib/apt/lists/*

ENV LANG=en_US.UTF-8
ENV LC_ALL=en_US.UTF-8

R
```

</details>
