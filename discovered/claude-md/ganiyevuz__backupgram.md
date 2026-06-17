---
name: ganiyevuz__backupgram
source: https://github.com/ganiyevuz/backupgram/blob/c24eb85d0f7f851d5947e0f773138b84fa049bb5/CLAUDE.md
repo: ganiyevuz/backupgram
kind: claude-md
stars: 3
last_pushed: 2026-06-07T04:41:22Z
license: mit
score: 9
domains: [devops, cli-tools, database]
tags: [bash, docker, postgres, automation]
curated: 2026-06-15
curated_by: config-scout
---

# ganiyevuz/backupgram — claude-md

**Why it's worth keeping:** It explicitly warns against editing generated files (docker-bake.hcl) and provides highly specific, copy-pasteable test commands that include necessary environment variables.

**Summary:** This file provides a deep dive into the container's runtime execution chain, environment variable resolution logic, and specific shell script nuances.

**Source credibility:** Low star count suggests a niche utility, but the documentation quality is professional and high-density.

**Recency:** Extremely current; recently pushed and reflects modern containerized CI/CD patterns.

**Source:** [ganiyevuz/backupgram/CLAUDE.md](https://github.com/ganiyevuz/backupgram/blob/c24eb85d0f7f851d5947e0f773138b84fa049bb5/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A Docker image (pure Bash, no application runtime) that runs automated PostgreSQL backups on a cron schedule, with rotating retention, Telegram delivery, optional GPG encryption, webhooks, and built-in restore tooling. Published as `ganiyevuz/backupgram:<pg-version>[-alpine]` for 4 PostgreSQL versions (15–18) × 2 base images (Debian/Alpine) × 2 platforms (amd64, arm64).

There is **no local build/lint/test toolchain** — everything is shell scripts baked into a Postgres-based image. Verification happens via the CI matrix (`.github/workflows/ci.yml`), which runs the scripts directly against a live `postgres:16` service container.

## Runtime architecture

The container entrypoint chain:

```
init.sh (ENTRYPOINT)
  └─ /env.sh            # standalone validation when VALIDATE_ON_START=TRUE
  └─ exec go-cron -s "$SCHEDULE" -- /backup.sh   # go-cron is the scheduler + healthcheck HTTP server
```

`go-cron` (downloaded from prodrigestivill/go-cron in the Dockerfile) owns the schedule and serves the healthcheck port. It invokes `backup.sh` per `SCHEDULE`.

**
```

</details>
