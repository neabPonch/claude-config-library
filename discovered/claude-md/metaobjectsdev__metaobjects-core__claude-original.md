---
name: metaobjectsdev__metaobjects-core__claude-original
source: https://github.com/metaobjectsdev/metaobjects-core/blob/37fef3bb1533cebd5d23ee255e63e29dbfe5db69/.claude/archive/CLAUDE.md.original
repo: metaobjectsdev/metaobjects-core
kind: claude-md
stars: 7
last_pushed: 2026-05-19T17:29:53Z
license: apache-2.0
score: 9
domains: [backend, java, system-architecture]
tags: [metadata, concurrency, design-patterns, caching]
curated: 2026-06-15
curated_by: config-scout
---

# metaobjectsdev/metaobjects-core — claude-md

**Why it's worth keeping:** Uses high-level analogies (ClassLoader) to establish mental models; provides explicit technical justifications for data structure choices like WeakHashMap vs ConcurrentHashMap.

**Summary:** Defines a read-optimized metadata architecture using Java Reflection analogies to enforce specific memory and concurrency patterns.

**Source credibility:** High technical density suggests professional engineering intent despite a smaller star count.

**Recency:** Highly relevant; follows modern standards for providing architectural guardrails to AI agents.

**Source:** [metaobjectsdev/metaobjects-core/.claude/archive/CLAUDE.md.original](https://github.com/metaobjectsdev/metaobjects-core/blob/37fef3bb1533cebd5d23ee255e63e29dbfe5db69/.claude/archive/CLAUDE.md.original) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MetaObjects Project - Claude AI Assistant Guide

## ⚠️ CRITICAL ARCHITECTURAL PRINCIPLE ⚠️

**MetaObjects follows a READ-OPTIMIZED WITH CONTROLLED MUTABILITY design pattern analogous to Java's Class/Field reflection system with dynamic class loading:**

- **MetaData objects are loaded once during application startup and optimized for heavy read access**
- **They are permanent in memory for the application lifetime (like Java Class objects)**
- **Thread-safe for concurrent READ operations (primary use case: 99.9% of operations)**
- **Support INFREQUENT controlled updates** (metadata repository pushes, dynamic editing)
- **Updates use Copy-on-Write patterns to maintain read performance during changes**
- **DO NOT treat MetaData as frequently mutable domain objects - optimize for heavy reads, rare updates**

### Framework Analogy
| Java Reflection | MetaObjects Framework | Dynamic Updates |
|----------------|----------------------|----------------|
| `Class.forName()` | `MetaDataLoader.load()` | `loader.reload()` |
| `Class.getFields()` | `MetaObject.getMetaFields()` | Copy-on-write fields |
| `Field.get(object)` | `MetaField.getValue(object)` | Read during update |
| Permanent in m
```

</details>
