---
name: OriNachum__autonomous-intelligence__memory-as-skill
source: https://github.com/OriNachum/autonomous-intelligence/blob/7f34d35030f36ee7a62c7fbab25446956053e524/qq/docs/memory-as-skill.md
repo: OriNachum/autonomous-intelligence
kind: skill
stars: 228
last_pushed: 2026-04-08T22:55:00Z
license: mit
score: 9
domains: [agents-ai, knowledge-management, backend-api]
tags: [memory, rag, neo4j, progressive-disclosure]
curated: 2026-06-14
curated_by: config-scout
---

# OriNachum/autonomous-intelligence — skill

**Why it's worth keeping:** Uses the pattern of linking to detailed reference docs in `references/` to prevent context bloat while providing deep API access. It effectively manages multiple backends (RAG, Graph, File Analysis) through a single unified skill interface.

**Summary:** A sophisticated blueprint for structuring complex, multi-layer agent skills using a 'progressive disclosure' architecture.

**Source credibility:** High-quality implementation from a highly-starred repository specializing in embodied AI.

**Recency:** Current; follows the latest Anthropic skills specification.

**Source:** [OriNachum/autonomous-intelligence/qq/docs/memory-as-skill.md](https://github.com/OriNachum/autonomous-intelligence/blob/7f34d35030f36ee7a62c7fbab25446956053e524/qq/docs/memory-as-skill.md) · 228★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Memory as Skill — Extraction Plan

**Goal**: Extract QQ's memory subsystems (notes core, notes ephemeral, MongoDB RAG, Neo4j knowledge graph) and `analyze_files` into a standalone, portable **skill** following the [Anthropic skills spec](https://github.com/anthropics/skills). JSON-based service configuration. Includes service initialization with partial setup support and configurable OpenAI-compatible endpoint.

---

## 1. Skill Structure

Following the official Anthropic skill anatomy: `SKILL.md` (required) + `scripts/`, `references/`, `assets/` (optional).

```
skills/memory/
├── SKILL.md                          # Frontmatter + concise workflow guide (<500 lines)
├── config.json                       # Service endpoints & credentials (user-editable)
├── config.sample.json                # Template with defaults
├── scripts/
│   ├── check_services.py             # Health-check all backends
│   ├── start_services.py             # docker-compose up (partial support)
│   ├── setup_openai.py               # Write OpenAI-compat config to config.json
│   └── migrate.py                    # Future: data migration between backends
├── references/
│   ├── notes-core.md                 #
```

</details>
