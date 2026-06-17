---
name: TuberculeP__Bloop
source: https://github.com/TuberculeP/Bloop/blob/1cb285817befafe0945fb4c23a595b25a3c5cc56/CLAUDE.md
repo: TuberculeP/Bloop
kind: claude-md
stars: 1
last_pushed: 2026-06-01T09:36:31Z
license: unknown
score: 7
domains: [web-frontend, fullstack]
tags: [hierarchical-documentation, project-mapping]
curated: 2026-06-16
curated_by: config-scout
---

# TuberculeP/Bloop — claude-md

**Why it's worth keeping:** Demonstrates an excellent hierarchical pattern for large codebases, preventing a single monolithic instruction file by delegating specific rules to relevant modules.

**Summary:** Acts as a central project index that routes the agent to specialized, module-specific CLAUDE.md files located in subdirectories.

**Source credibility:** Small-scale open-source project/personal repository.

**Recency:** Current; uses modern tech stacks like Vue 3 and Vite.

**Source:** [TuberculeP/Bloop/CLAUDE.md](https://github.com/TuberculeP/Bloop/blob/1cb285817befafe0945fb4c23a595b25a3c5cc56/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Bloop - Documentation Projet

> DAW collaboratif web avec réseau social intégré.

## Stack technique

| Couche | Technologie |
|--------|-------------|
| Frontend | Vue 3 + Pinia + TypeScript + SCSS |
| Backend | Express.js + TypeORM + PostgreSQL |
| Storage | Cloudflare R2 (S3-compatible) |
| Cache audio | IndexedDB (500MB, LRU) |
| Auth | Session-based + Google OAuth |

## Structure

```
pie-poc-2/
├── webapp/                    # Frontend Vue 3
│   └── src/
│       ├── components/app/    # DAW (voir CLAUDE.md)
│       ├── views/admin/       # Admin (voir CLAUDE.md)
│       └── stores/            # Pinia stores
├── server/                    # Backend Express
│   └── src/
│       ├── config/entities/   # Entités TypeORM
│       └── routes/            # API REST
└── CLAUDE.md
```

## Documentation par module

| Module | Fichier | Description |
|--------|---------|-------------|
| DAW Timeline | `webapp/src/components/app/CLAUDE.md` | Piano roll, pistes, engines audio |
| Piano Roll | `webapp/src/components/app/timeline/PianoRoll/CLAUDE.md` | Éditeur de notes |
| Admin | `webapp/src/views/admin/CLAUDE.md` | Gestion users + samples |

## Commandes

```bash
# Dev (depuis racine)
np
```

</details>
