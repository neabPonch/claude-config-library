---
name: Prismer-AI__Prismer
source: https://github.com/Prismer-AI/Prismer/blob/2dbe71feebeb53e2a54c708cac676835e08c2f24/CLAUDE.md
repo: Prismer-AI/Prismer
kind: claude-md
stars: 782
last_pushed: 2026-06-10T04:36:23Z
license: other
score: 9
domains: [web-frontend, agents-ai, system-architecture, docker]
tags: [architectural-patterns, state-management, agent-sync, fullstack]
curated: 2026-06-14
curated_by: config-scout
---

# Prismer-AI/Prismer — claude-md

**Why it's worth keeping:** Exemplary documentation of cross-layer data flows (Sync Layer/Directive Protocol) and specific state management patterns (Zustand store composition). It provides an LLM with the exact mental model required to extend high-concurrency synchronization logic without breaking the system.

**Summary:** A deep architectural blueprint that explains not just the 'what' but the 'how' of a complex multi-agent system.

**Source credibility:** High; established open-source project with significant star count and recent activity.

**Recency:** 

**Source:** [Prismer-AI/Prismer/CLAUDE.md](https://github.com/Prismer-AI/Prismer/blob/2dbe71feebeb53e2a54c708cac676835e08c2f24/CLAUDE.md) · 782★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Prismer.AI is an open-source academic research platform combining paper reading, writing, data analysis, and multi-agent AI workflows. It ships as a self-hosted Docker container with a Next.js frontend and uses OpenClaw for agent orchestration.

**Licensing:** Workspace (`web/`) and Docker (`docker/`) are Apache-2.0.

## Repository Structure

```
web/                     # Next.js 16 frontend (React 19, TypeScript, Tailwind 4)
docker/                  # Container infrastructure & OpenClaw integration
  base/                  # Base Docker image (ubuntu + LaTeX/Jupyter/Prover services)
  plugin/                # OpenClaw plugins (prismer-im, prismer-workspace)
  gateway/               # Container reverse proxy (zero-dependency)
  config/                # Agent config (openclaw.json, SOUL.md, AGENTS.md)
  templates/             # Agent personality templates (mathematician, finance, etc.)
  scripts/               # Python CLI tools (latex, jupyter, component, sync)
docs/                    # Architecture docs, roadmap, i18n translations
skills/
```

</details>
