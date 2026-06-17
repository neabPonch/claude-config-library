---
name: realgenekim__clj-surgeon
source: https://github.com/realgenekim/clj-surgeon/blob/6baa2a4dddc32f8cf5c7f86106beb0ed13c1deb0/skill.md
repo: realgenekim/clj-surgeon
kind: skill
stars: 29
last_pushed: 2026-06-11T23:06:36Z
license: mit
score: 9
domains: [cli-tools, clojure, refactoring]
tags: [ast, structural-editing, babashka]
curated: 2026-06-15
curated_by: config-scout
---

# realgenekim/clj-surgeon — skill

**Why it's worth keeping:** It demonstrates the pattern of augmenting an agent with domain-specific tools to handle high-risk structural transformations that standard text editing cannot safely execute.

**Summary:** A specialized toolkit for structural Clojure refactoring via a Babashka CLI, enabling complex AST-based operations like form extraction and CLJC merging.

**Source credibility:** Highly credible; features active maintenance and extensive test coverage (103 tests).

**Recency:** Extremely current, utilizing modern Babashka and Clojure patterns.

**Source:** [realgenekim/clj-surgeon/skill.md](https://github.com/realgenekim/clj-surgeon/blob/6baa2a4dddc32f8cf5c7f86106beb0ed13c1deb0/skill.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: clj-surgeon
description: "Clojure structural ops: outline, extract to new ns, fix-declares, deps tree, topo sort, form move, namespace rename, CLJC merge/split/add-require/analyze — babashka + rewrite-clj"
user-invocable: true
---

# clj-surgeon: Structural Operations on Clojure Namespaces

A babashka CLI tool at `~/bin/clj-surgeon`. Source at `~/src.local/clj-surgeon/`. 103 tests, 327 assertions.

## When to Use

- **Before exploring ANY Clojure codebase** — `:ls-tree` maps an entire directory of repos in seconds. "Which repo does X?" answered in one command instead of spawning Explore agents
- **Before reading a large .clj/.cljs/.cljc file** — `:ls` first (50 tokens vs 2000+); the outline now surfaces forms inside `#?(:clj …)` / `#?@(:cljs […])` with `:platforms` tags
- **When searching across multiple repos** — `:ls-tree :grep "pattern"` finds matching projects/files with full API surface, ~3 seconds across thousands of files
- **When extracting forms to a new namespace** — `:extract!` does it in one command
- **When you see a `declare`** — `:fix-declares!` eliminates removable ones
- **When reordering forms** — `:mv` moves a defn above its caller
- **When renaming a n
```

</details>
