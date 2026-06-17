---
name: misprit7__mtgenv
source: https://github.com/misprit7/mtgenv/blob/a96a7d9de91c5f630842b0e62460d0796edbad9d/CLAUDE.md
repo: misprit7/mtgenv
kind: claude-md
stars: 0
last_pushed: 2026-06-14T13:25:22Z
license: unknown
score: 9
domains: [systems-programming, game-engine]
tags: [architecture-centric, context-hierarchy, strict-constraints]
curated: 2026-06-14
curated_by: config-scout
---

# misprit7/mtgenv — claude-md

**Why it's worth keeping:** Uses 'Architecture laws' to prevent scope creep/drift and provides a structured way for the AI to consume context through prioritized documentation.

**Summary:** Defines strict architectural constraints, a documentation hierarchy via 'Read order', and specific project state maintenance procedures.

**Source credibility:** Single-author repo with high technical density suggesting expert domain knowledge.

**Recency:** Current; includes modern Rust testing and development practices.

**Source:** [misprit7/mtgenv/CLAUDE.md](https://github.com/misprit7/mtgenv/blob/a96a7d9de91c5f630842b0e62460d0796edbad9d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — mtgenv

Guidance for AI agents (and humans) working in this repo. Read this first.

## What this is

`mtgenv` is a **from-scratch Rust implementation of the Magic: The Gathering rules
engine**, intended to be the fast, headless simulation core of a **Gymnasium RL
environment** for training an MTG AI in Python + PyTorch (self-play). Long-term it should
implement the full ruleset; near-term it's a tiny card pool with a correct core.

## Setup

After cloning, run `./scripts/setup.sh` once (idempotent). It downloads Scryfall's
`default_cards` bulk data (one object per printing, so every Arena printing's `arena_id`
is present) into the gitignored `data/scryfall/` and installs the web client's npm deps.
Then `cargo build` / `cargo test`.

## Read order (the docs are the spec & the plan)

1. `docs/design/WHITEBOARD_MODEL.md` — **the architecture.** The engine is modeled on MTG
   Arena's own "whiteboard" GRE design. This is a deliberate, load-bearing decision.
2. `docs/rules/RULES_SUMMARY.md` — engine-implementer's map of the Comprehensive Rules,
   with CR rule numbers. The raw rules are in `docs/rules/comprules.txt` (grep by number,
   e.g. `613.` for the layer system) and
```

</details>
