---
name: langchain-ai__docs
source: https://github.com/langchain-ai/docs/blob/2122d9ec64415e55c284b83805e35ba49c693714/CLAUDE.md
repo: langchain-ai/docs
kind: claude-md
stars: 360
last_pushed: 2026-06-15T03:26:12Z
license: mit
score: 9
domains: [documentation, web-content]
tags: [mdx, mintlify, seo, structured-docs]
curated: 2026-06-15
curated_by: config-scout
---

# langchain-ai/docs — claude-md

**Why it's worth keeping:** Uses high-density 'Never' constraints to prevent SEO/build errors and includes a detailed navigation map to ensure correct file placement in complex structures.

**Summary:** Provides exhaustive guidelines for authoring, structuring, and navigating documentation within a Mintlify/MDX-based system.

**Source credibility:** High; LangChain is an industry-standard AI framework with a highly active repository.

**Recency:** Current; the project shows extremely recent maintenance activity.

**Source:** [langchain-ai/docs/CLAUDE.md](https://github.com/langchain-ai/docs/blob/2122d9ec64415e55c284b83805e35ba49c693714/CLAUDE.md) · 360★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
> **Keep in sync:** `AGENTS.md` and `CLAUDE.md` contain identical guidelines. If you update one, update the other.

# LangChain Documentation Guidelines

Documentation for LangChain products hosted on Mintlify. These guidelines apply to manually authored content under `src/`, not Mintlify `build/` output.

## Critical rules

1. **Always ask for clarification** rather than making assumptions
2. **Never fabricate** examples, JSON snippets, policy details, or use case descriptions — use only content from the user or existing source files
3. **Never use markdown in frontmatter `description`** — breaks SEO
4. **Never edit `build/`** — Mintlify build output (regenerate with `make build` or `make dev`)
5. **Always update `src/docs.json`** when adding new pages
6. **Use Tabler icons only** — not FontAwesome
7. **Test code examples** before including them

## Quick reference

| What | Where/How |
|------|-----------|
| LangSmith docs | `src/langsmith/` |
| Open source docs | `src/oss/` (LangChain, LangGraph, Deep Agents) |
| Python integrations | `src/oss/python/integrations/` |
| JS integrations | `src/oss/javascript/integrations/` |
| Reusable snippets | `src/snippets/` |
| Images | `src/
```

</details>
