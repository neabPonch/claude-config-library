---
name: FgForrest__evitaDB__skill
source: https://github.com/FgForrest/evitaDB/blob/7d18a9b37a8e77cfdf79e45e5da28c6dc28bb8a7/.claude/skills/new-external-api-object/SKILL.md
repo: FgForrest/evitaDB
kind: skill
stars: 67
last_pushed: 2026-06-10T10:39:16Z
license: other
score: 9
domains: [backend-api, distributed-systems]
tags: [schema-design, api-contract, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# FgForrest/evitaDB — skill

**Why it's worth keeping:** The file includes a detailed module map and clarifies complex inheritance rules (from vs. implementing) that are critical for maintaining cross-API consistency.

**Summary:** Provides highly technical instructions for adding new response objects across GraphQL, REST, and gRPC APIs using a custom descriptor-based architecture.

**Source credibility:** High; comes from a specialized database project with recent maintenance activity.

**Recency:** Recent; uses modern architectural patterns suitable for current development workflows.

**Source:** [FgForrest/evitaDB/.claude/skills/new-external-api-object/SKILL.md](https://github.com/FgForrest/evitaDB/blob/7d18a9b37a8e77cfdf79e45e5da28c6dc28bb8a7/.claude/skills/new-external-api-object/SKILL.md) · 67★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: new-external-api-object
description: Use when adding a new response object (DTO surface) to evitaDB's external APIs — GraphQL, REST, and gRPC. Covers descriptors and their inheritance, interfaces and field-override rules, per-parameter object caches, GraphQL data fetchers, and gRPC proto/converter patterns with backward-compat rules. Use this whenever introducing a new object type, a suffix variant, or a polymorphic interface that must be exposed via at least two of the three APIs.
---

# Adding a new external API object

evitaDB projects every response object through three external APIs — GraphQL, REST (OpenAPI), gRPC. All three share a single API-independent model in `evita_external_api_core` called **descriptors**, then each API module translates those descriptors into its own runtime types.

Use this skill when:
- Introducing a brand-new response object that is not yet exposed.
- Adding a new suffix variant of an existing object (e.g. `withHistograms` alongside the regular form).
- Refactoring an existing concrete object into an **interface + implementations** polymorphic shape.

## Module map

```
evita_external_api_core/          descriptors (API-independent)
└─ ...
```

</details>
