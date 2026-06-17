---
name: cachix__devenv__skill
source: https://github.com/cachix/devenv/blob/48a93d1fd74ca3fb4f3f64e942cfcb19a1d9f7e0/.agents/skills/create-service/SKILL.md
repo: cachix/devenv
kind: skill
stars: 6997
last_pushed: 2026-06-14T16:56:31Z
license: apache-2.0
score: 9
domains: [devops, infrastructure-as-code, nix, backend-orchestration]
tags: [service-modules, nix-devenv, process-management]
curated: 2026-06-15
curated_by: config-scout
---

# cachix/devenv — skill

**Why it's worth keeping:** It moves beyond syntax to define advanced orchestration patterns like readiness probes, systemd notify/watchdog protocols, and task-based initialization DAGs. The emphasis on Unix sockets over TCP and dynamic port allocation is a high-level architectural pattern worth stealing.

**Summary:** A highly structured skill for generating service modules within a 'devenv' Nix-based environment. It provides rigorous architectural standards for port allocation, socket activation, and lifecycle management.

**Source credibility:** Very high; cachix/devenv is a major, highly-starred project in the Nix ecosystem.

**Recency:** Highly current; source was updated recently.

**Source:** [cachix/devenv/.agents/skills/create-service/SKILL.md](https://github.com/cachix/devenv/blob/48a93d1fd74ca3fb4f3f64e942cfcb19a1d9f7e0/.agents/skills/create-service/SKILL.md) · 6997★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: create-service
description: This skill should be used when the user asks to "create a service module", "add a new service", "write a service for", "implement a service module", or wants to add a new service to src/modules/services/. Provides the patterns and conventions for devenv service modules.
argument-hint: [service-name]
---

# Create a devenv Service Module

This skill guides the creation of new service modules under `src/modules/services/`.

## Process

1. Research the service: default port, package name in nixpkgs, config file format, socket activation support, systemd notify/watchdog support
2. Read existing modules in `src/modules/services/` for reference (e.g., `memcached.nix` for simple, `redis.nix` for medium, `minio.nix` for complex)
3. Create `src/modules/services/<name>.nix` following the patterns below (auto-discovered)
4. Add a test under `tests/`

## Unix Sockets Preferred

When a service supports unix sockets, prefer them over TCP ports as the default communication method. Unix sockets are faster, avoid port conflicts, and are more secure for local-only services. See `redis.nix` for the pattern: use `DEVENV_RUNTIME` for the socket path, expose `$<NAME
```

</details>
