---
name: nuxt-modules__og-image__skill
source: https://github.com/nuxt-modules/og-image/blob/26183703e95620df5aa0daf01a5cf98df3a50274/.claude/skills/takumi-rs-core-skilld/SKILL.md
repo: nuxt-modules/og-image
kind: skill
stars: 539
last_pushed: 2026-06-12T07:48:21Z
license: mit
score: 9
domains: [web-frontend, performance-optimization, developer-tools]
tags: [library-specific, breaking-changes, best-practices]
curated: 2026-06-16
curated_by: config-scout
---

# nuxt-modules/og-image — skill

**Why it's worth keeping:** The inclusion of a dedicated 'Breaking Changes' section is a top-tier technique for preventing LLM regressions during refactors. The specific technical advice (e.g., TTF vs WOFF2 or Renderer reuse) provides high-signal, non-obvious architectural guidance.

**Summary:** A highly specialized context file for the `@takumi-rs/core` library that details breaking changes, new APIs, and performance optimizations. It also introduces a structured `skilld search` pattern to help an agent navigate documentation efficiently.

**Source credibility:** High; the structure demonstrates an advanced understanding of how to augment agent knowledge via highly dense, actionable documentation summaries.

**Recency:** Very current, focusing on modern edge/WASM runtimes and specialized environment detection.

**Source:** [nuxt-modules/og-image/.claude/skills/takumi-rs-core-skilld/SKILL.md](https://github.com/nuxt-modules/og-image/blob/26183703e95620df5aa0daf01a5cf98df3a50274/.claude/skills/takumi-rs-core-skilld/SKILL.md) · 539★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: takumi-rs-core-skilld
description: "ALWAYS use when writing code importing \"@takumi-rs/core\". Consult for debugging, best practices, or modifying @takumi-rs/core, takumi-rs/core, takumi-rs core, takumi rs core, takumi."
metadata:
  version: 1.0.0-beta.3
  generated_by: Claude Code · Haiku 4.5
  generated_at: 2026-03-17
---

# kane50613/takumi `@takumi-rs/core`

**Version:** 1.0.0-beta.3
**Deps:** @takumi-rs/helpers@0.73.1
**Tags:** latest: 0.73.1, beta: 1.0.0-beta.3

**References:** [package.json](./.skilld/pkg/package.json) — exports, entry points • [README](./.skilld/pkg/README.md) — setup, basic usage • [Docs](./.skilld/docs/_INDEX.md) — API reference, guides • [GitHub Issues](./.skilld/issues/_INDEX.md) — bugs, workarounds, edge cases • [GitHub Discussions](./.skilld/discussions/_INDEX.md) — Q&A, patterns, recipes • [Releases](./.skilld/releases/_INDEX.md) — changelog, breaking changes, new APIs

## Search

Use `skilld search` instead of grepping `.skilld/` directories — hybrid semantic + keyword search across all indexed docs, issues, and releases. If `skilld` is unavailable, use `npx -y skilld search`.

```bash
skilld search "query" -p @takumi-rs/core
skilld searc
```

</details>
