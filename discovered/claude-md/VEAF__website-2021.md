---
name: VEAF__website-2021
source: https://github.com/VEAF/website-2021/blob/485f63fd9851107bfa85286528291187f89977a0/CLAUDE.md
repo: VEAF/website-2021
kind: claude-md
stars: 3
last_pushed: 2026-02-11T18:51:46Z
license: unknown
score: 9
domains: [backend, php-symfony, devops]
tags: [symfony, testing-patterns, docker-workflow, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# VEAF/website-2021 — claude-md

**Why it's worth keeping:** It provides concrete code examples for different test types (Unit vs Integration) and explicitly defines the business domain to prevent semantic errors. The emphasis on using project-specific shell scripts over raw commands is an excellent pattern for AI efficiency.

**Summary:** A highly detailed guide that covers specific command-line workflows via scripts and explains a complex dual-database architecture.

**Source credibility:** Small community repo, but the level of detail suggests a professional developer's workflow.

**Recency:** Very current; the content is highly relevant to modern Claude Code interactions.

**Source:** [VEAF/website-2021/CLAUDE.md](https://github.com/VEAF/website-2021/blob/485f63fd9851107bfa85286528291187f89977a0/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

VEAF Website is a Symfony PHP application for the Virtual European Air Force (VEAF) flight simulation community. It was also configurable for 51ème Escadron Griffon (51eg) via the `WEBSITE` environment variable.

## Development Commands

All commands use Docker and are run via shell scripts in `./scripts/`:

```bash
./scripts/upgrade.sh       # Pull images, start containers, install composer deps, run migrations
./scripts/dev/fixtures.sh  # Load test fixtures (requires `touch .fixtures` safety file)
./scripts/start.sh         # Start all containers
./scripts/stop.sh          # Stop all containers
./scripts/php.sh           # Shell into PHP container as www-data (or run a command)
./scripts/console.sh       # Run Symfony console commands
./scripts/cc.sh            # Clear Symfony cache
./scripts/fix.sh           # Run PHP CS Fixer on src/
./scripts/dev/test.sh      # Run tests
```

All scripts support `--help` for detailed usage information.

Console commands (via `./scripts/console.sh`):
```bash
./scripts/console.sh doctrine:migrations:migrate -n
```

</details>
