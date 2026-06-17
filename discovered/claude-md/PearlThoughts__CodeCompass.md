---
name: PearlThoughts__CodeCompass
source: https://github.com/PearlThoughts/CodeCompass/blob/24ebf13c30d48e3c19f3e662baf7f34118e0b73d/Claude.md
repo: PearlThoughts/CodeCompass
kind: claude-md
stars: 1
last_pushed: 2025-11-25T13:46:00Z
license: other
score: 9
domains: [backend-api, ai-agents, cli-tools]
tags: [capabilities-map, skill-based-workflows, context-management, nest-js]
curated: 2026-06-14
curated_by: config-scout
---

# PearlThoughts/CodeCompass — claude-md

**Why it's worth keeping:** The tiered approach of mapping capabilities via JSON and providing on-demand specialized 'skills' (markdown files) is a world-class pattern for managing context in large codebases.

**Summary:** Combines deep architectural documentation with a sophisticated 'AI Context System' using capability maps and specialized skill files.

**Source credibility:** High-quality, enterprise-grade documentation from an active project with clear architectural rigor.

**Recency:** Very current; specifically optimized for managing token costs and agentic workflows.

**Source:** [PearlThoughts/CodeCompass/Claude.md](https://github.com/PearlThoughts/CodeCompass/blob/24ebf13c30d48e3c19f3e662baf7f34118e0b73d/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CodeCompass Project Documentation

## Project Overview

CodeCompass is an enterprise-grade code intelligence platform for analyzing and modernizing large-scale codebases. The system provides semantic search, AST analysis, requirements extraction, and automated migration support through a vector database-powered architecture.

**Project Location**: `/Users/SenG/Projects/CodeCompass`
**Origin**: Extracted from `/Users/SenG/Projects/Compass` monorepo (2024-11-22)
**Status**: Independent standalone project
**Version**: 1.0.0

---

## System Architecture

### Technology Stack

- **Framework**: NestJS (TypeScript)
- **Database**: PostgreSQL + TypeORM
- **Vector Database**: Weaviate
- **Queue System**: Bull + Redis
- **CLI Framework**: nest-commander
- **Testing**: Vitest
- **Embeddings**: Ollama (local inference)

### Infrastructure Configuration

All infrastructure services run locally within this project directory. No external dependencies or shared resources with other projects.

**Docker Services** (`docker-compose up -d`):
```
codecompass-postgres   → localhost:5433
codecompass-redis      → localhost:6380
codecompass-weaviate   → localhost:8081
```

**Ollama** (native macOS servic
```

</details>
