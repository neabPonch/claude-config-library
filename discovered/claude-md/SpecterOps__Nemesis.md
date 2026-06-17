---
name: SpecterOps__Nemesis
source: https://github.com/SpecterOps/Nemesis/blob/432d08157d011f811d67591b55c229aa54b79309/CLAUDE.md
repo: SpecterOps/Nemesis
kind: claude-md
stars: 972
last_pushed: 2026-05-22T01:17:59Z
license: bsd-3-clause
score: 9
domains: [backend-api, security, microservices, devops]
tags: [operational-commands, architecture-map, security-guardrails]
curated: 2026-06-14
curated_by: config-scout
---

# SpecterOps/Nemesis — claude-md

**Why it's worth keeping:** Includes critical security guardrails (blocking .env access), provides a visual directory tree/data-flow map, and defines specific testing philosophies like mocking external services.

**Summary:** A comprehensive operational guide for a complex microservices architecture, covering deployment, development workflows, and data flow.

**Source credibility:** High; authored by SpecterOps, a recognized leader in offensive security operations.

**Recency:** Current; utilizes modern tooling such as 'uv' and Python 3.13.

**Source:** [SpecterOps/Nemesis/CLAUDE.md](https://github.com/SpecterOps/Nemesis/blob/432d08157d011f811d67591b55c229aa54b79309/CLAUDE.md) · 972★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## File Restrictions

**NEVER read, open, or access `.env` files under any circumstances.** This includes:
- `.env`
- `.env.local`
- `.env.development`
- `.env.production`
- Any file matching the pattern `.env*`

If you need environment variable information, refer to `env.example` instead.

## Project Overview

Nemesis is an open-source, centralized data processing platform (v2.0) that ingests, enriches, and enables collaborative analysis of files collected during offensive security assessments. Built on Docker with Dapr integration, it functions as an "offensive VirusTotal."

## Common Commands

### Running Nemesis

```bash
# Start production services
./tools/nemesis-ctl.sh start prod

# Start with monitoring, jupyter, and LLM support
./tools/nemesis-ctl.sh start prod --monitoring --jupyter --llm

# Start development environment (always builds)
./tools/nemesis-ctl.sh start dev

# Stop services (use same flags as start)
./tools/nemesis-ctl.sh stop prod --monitoring --jupyter --llm

# Stop and remove volumes
./tools/nemesis-ctl.sh clean prod --monitoring --jupyter --l
```

</details>
