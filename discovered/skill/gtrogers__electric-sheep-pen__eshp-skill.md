---
name: gtrogers__electric-sheep-pen__eshp-skill
source: https://github.com/gtrogers/electric-sheep-pen/blob/57d97a264fedfed47bd7e3a878cba362c3cb1781/eshp-skill.md
repo: gtrogers/electric-sheep-pen
kind: skill
stars: 4
last_pushed: 2026-06-11T12:11:11Z
license: mit
score: 8
domains: [agents-ai, cli-tools, knowledge-management, developer-experience]
tags: [memory-graph, context-management, structured-notes, graph-theory]
curated: 2026-06-15
curated_by: config-scout
---

# gtrogers/electric-sheep-pen — skill

**Why it's worth keeping:** Uses structured relationship types (.rel-name) to enable graph traversal instead of just full-text search; maintains Git-friendly text files for shared team memory.

**Summary:** A codebase-local knowledge graph system that uses plain-text files and typed edges to store architectural decisions and concept relationships. It allows an agent to build and traverse a structured mental model of a repository.

**Source credibility:** Niche/specialized tool with high utility for the emerging 'agentic memory' problem.

**Recency:** Highly current; solves a fundamental limitation in modern LLM coding workflows regarding long-term context.

**Source:** [gtrogers/electric-sheep-pen/eshp-skill.md](https://github.com/gtrogers/electric-sheep-pen/blob/57d97a264fedfed47bd7e3a878cba362c3cb1781/eshp-skill.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# eshp — agent skill

## What it is

`memo` is a codebase-local knowledge graph. Notes live as plain-text `.eshp`
files in a `eshp/` folder; a SQLite graph index (`.eshp.db`) is kept in sync by
a background watcher or on-demand sync. Use it to record observations,
decisions, warnings, and typed relationships between concepts in the codebase.

## When to use it

| Situation | Action |
|-----------|--------|
| Starting a session on an unfamiliar codebase | `eshp search <topic>` to surface prior context |
| You learn something worth remembering | `eshp new <slug>` to create a note |
| Two concepts are related | `eshp relate` (write edge into the `.eshp` file) or edit directly |
| Exploring how things connect | `eshp graph <slug> --depth 2` |
| Recalling what exists in a domain | `eshp tag <tagname>` or `eshp tags` |

---

## Command reference

### Watch (recommended — run in background)
```
eshp watch [--root PATH]
```
Bootstraps the DB from all `.eshp` files then watches for changes. Keep this
running so every file edit is indexed immediately.

### Create a note
```
eshp new <slug> [--tags tag1,tag2] [--root PATH]
```
Creates `eshp/<slug>.eshp`, opens it in `$EDITOR`, and syncs on sa
```

</details>
