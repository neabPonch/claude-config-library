---
name: kool-dev__kool__skill
source: https://github.com/kool-dev/kool/blob/f2d9701be3dbd43c8301d26d43053a4b1aabb3b3/skills/kool-cli/SKILL.md
repo: kool-dev/kool
kind: skill
stars: 722
last_pushed: 2026-04-22T03:01:07Z
license: mit
score: 8
domains: [cli-tools, devops, docker]
tags: [container-orchestration, development-workflow, docker-compose]
curated: 2026-06-15
curated_by: config-scout
---

# kool-dev/kool — skill

**Why it's worth keeping:** The inclusion of an 'Important Rules' section provides crucial constraints that prevent agent errors when executing scripts or navigating directories.

**Summary:** A comprehensive command-line reference manual for the 'kool' CLI tool used to manage Dockerized development environments.

**Source credibility:** High; a well-starred (722) and recently maintained developer tool.

**Recency:** Current; highly compatible with modern agentic workflows for infrastructure management.

**Source:** [kool-dev/kool/skills/kool-cli/SKILL.md](https://github.com/kool-dev/kool/blob/f2d9701be3dbd43c8301d26d43053a4b1aabb3b3/skills/kool-cli/SKILL.md) · 722★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kool-cli
description: Docker development environment CLI. Use for managing containers (start/stop/restart), executing commands in services, viewing logs, and running project scripts from kool.yml.
---

# Kool CLI

Kool simplifies Docker-based development with commands for container lifecycle, service execution, and custom scripts.

## Quick Reference

```bash
kool start                    # Start all services from docker-compose.yml
kool stop                     # Stop all services
kool restart --rebuild        # Restart and rebuild images
kool status                   # Show running containers
kool exec <service> <cmd>     # Run command in service container
kool logs -f <service>        # Follow service logs
kool run --json               # List available scripts as JSON
kool run <script>             # Run a script from kool.yml
```

## Service Lifecycle

Services are defined in `docker-compose.yml`. Kool wraps docker-compose with simpler commands.

```bash
kool start                    # Start all services
kool start app database       # Start specific services
kool start --rebuild          # Rebuild images before starting
kool start --foreground       # Run in foregroun
```

</details>
