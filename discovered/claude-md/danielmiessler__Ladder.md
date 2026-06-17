---
name: danielmiessler__Ladder
source: https://github.com/danielmiessler/Ladder/blob/7f8ca3c28351adb270d35c0496744fd90230eb69/CLAUDE.md
repo: danielmiessler/Ladder
kind: claude-md
stars: 229
last_pushed: 2026-03-22T19:54:18Z
license: mit
score: 8
domains: [cli-tools, knowledge-management]
tags: [protocol, workflow, structured-data]
curated: 2026-06-15
curated_by: config-scout
---

# danielmiessler/Ladder — claude-md

**Why it's worth keeping:** Implements strict naming/ID patterns to prevent data corruption and provides explicit command-line constraints to ensure the AI uses the correct runtime (Bun) over defaults.

**Summary:** Defines a high-context protocol for a closed-loop experimental pipeline using structured markdown and specific ID conventions.

**Source credibility:** High; authored by Daniel Miessler, a prominent figure in security and information theory.

**Recency:** Current; updated within the last few months.

**Source:** [danielmiessler/Ladder/CLAUDE.md](https://github.com/danielmiessler/Ladder/blob/7f8ca3c28351adb270d35c0496744fd90230eb69/CLAUDE.md) · 229★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Ladder — AI Guidance

## What Is This?

Ladder is an open source pipeline for systematic improvement: Sources → Ideas → Hypotheses → Experiments → Results, with results feeding back as sources (the loop).

## Key Conventions

- **IDs**: Each collection uses a prefix: `SR-`, `ID-`, `HY-`, `EX-`, `AL-`, `RE-` followed by 5-digit zero-padded number
- **Format**: All entries are markdown with YAML frontmatter
- **Status values**: `draft`, `active`, `testing`, `complete`, `archived`
- **Linking**: Entries reference upstream items (e.g., a hypothesis links to its parent idea via `idea: ID-00001`)
- **CLI**: Use `bun run ladder <command>` — never npm/npx

## Directory Structure

- `Sources/` — Raw inputs (papers, articles, observations, telemetry)
- `Ideas/` — Candidate solutions generated from sources
- `Hypotheses/` — Testable predictions from ideas
- `Experiments/` — Structured tests with methodology
- `Algorithms/` — Proven methods for specific tasks
- `Results/` — Verified outcomes from experiments
- `Tools/` — TypeScript CLI tooling (bun-based)

## When Adding Entries

1. Use the CLI: `bun run ladder add <type> --title "..."`
2. Or create manually following the TEMPLATE.md in each
```

</details>
