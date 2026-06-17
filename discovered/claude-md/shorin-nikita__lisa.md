---
name: shorin-nikita__lisa
source: https://github.com/shorin-nikita/lisa/blob/9708c068f7635bb64241bd0078cc51ecff045f4a/CLAUDE.md
repo: shorin-nikita/lisa
kind: claude-md
stars: 80
last_pushed: 2026-03-13T17:24:12Z
license: apache-2.0
score: 9
domains: [devops, ai-infrastructure, docker]
tags: [docker-compose, n8n, deployment-automation, self-hosted]
curated: 2026-06-15
curated_by: config-scout
---

# shorin-nikita/lisa — claude-md

**Why it's worth keeping:** It highlights critical 'gotchas' like mandatory project name flags (`-p localai`) to maintain network connectivity across merged compose files and details precise startup/update sequences.

**Summary:** This file provides deep architectural context for managing a complex multi-container AI stack, covering deployment, hardware profiles, and service dependencies.

**Source credibility:** Solid mid-sized open-source project with active maintenance and clear technical documentation.

**Recency:** Very recent; utilizes modern Docker features like the 'include' directive and profiles.

**Source:** [shorin-nikita/lisa/CLAUDE.md](https://github.com/shorin-nikita/lisa/blob/9708c068f7635bb64241bd0078cc51ecff045f4a/CLAUDE.md) · 80★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

# Л.И.С.А. — Локальная Интеллектуальная Система Автоматизации

Self-hosted AI platform combining N8N automation, Supabase database, Ollama LLMs, Whisper speech recognition, and media processing in a unified Docker Compose stack.

## Core Architecture

### Multi-Compose Stack Pattern

The project uses a **unified Docker Compose architecture** with two separate compose files merged under one project:

1. **Main stack** (`docker-compose.yml`) — AI services (N8N, Ollama, Whisper, Qdrant, etc.)
2. **Supabase stack** (`supabase/docker/docker-compose.yml`) — Full Supabase suite included via `include:` directive
3. **All services share**:
   - Single Docker network: `localai_default`
   - Single project name: `localai`
   - Single `.env` file (copied to `supabase/docker/.env` by startup script)

**Critical**: Never use separate project names. All `docker compose` commands MUST use `-p localai` to maintain service connectivity.

### GPU Profile System

Ollama uses Docker Compose profiles to support different hardware:

- `cpu` → `ollama-cpu` service (no GPU acceleration)
```

</details>
