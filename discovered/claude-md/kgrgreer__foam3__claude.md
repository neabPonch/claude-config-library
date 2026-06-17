---
name: kgrgreer__foam3__claude
source: https://github.com/kgrgreer/foam3/blob/0c24834f3876975efeb143a4b6c228973552409e/doc/guides/claude.md
repo: kgrgreer/foam3
kind: claude-md
stars: 49
last_pushed: 2026-06-16T01:26:19Z
license: other
score: 8
domains: [framework-design, dsls, architectural-patterns]
tags: [model-driven, dsl, philosophy]
curated: 2026-06-16
curated_by: config-scout
---

# kgrgreer/foam3 — claude-md

**Why it's worth keeping:** It encodes a specific architectural paradigm ('code is a liability') that prevents LLMs from attempting manual implementation instead of using the required DSL/model approach.

**Summary:** Defines the philosophical and structural rules of the FOAM model-driven framework.

**Source credibility:** Niche, highly specialized project with high technical density; 49 stars suggests a focused community.

**Recency:** Current; utilizes modern JavaScript syntax and reflects contemporary architectural patterns.

**Source:** [kgrgreer/foam3/doc/guides/claude.md](https://github.com/kgrgreer/foam3/blob/0c24834f3876975efeb143a4b6c228973552409e/doc/guides/claude.md) · 49★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FOAM for LLMs

> FOAM (Feature-Oriented Active Modeller) is a model-driven, cross-platform application framework for JavaScript, Java, and Swift. Everything is a model. Everything is composable. Code is a liability; declarations are assets.

---

## 1. Why FOAM Works — Design Philosophy

Many model-driven frameworks have been attempted. Most collapse under their own weight. Understanding why FOAM is different shapes how you should write FOAM code.

**Code is a liability, not an asset.** The asset is the *feature*. Code is the maintenance burden you pay to have the feature. FOAM's goal is to minimise that burden by generating as much code as possible at build or runtime — code that is never edited and never checked in. When you find yourself writing boilerplate in FOAM, that is a signal that something should be declared or generated instead.

**Generated code is never edited.** Classic code generators produced a starting point that developers would then modify — which meant the generator and the code immediately diverged. FOAM avoids this entirely. Model definitions are the source of truth; everything derived from them is regenerated. This is the only way the model stays authorita
```

</details>
