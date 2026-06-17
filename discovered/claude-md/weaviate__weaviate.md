---
name: weaviate__weaviate
source: https://github.com/weaviate/weaviate/blob/24163aff9ea6af1ca80a74e8ecf10f6a81ae689f/CLAUDE.md
repo: weaviate/weaviate
kind: claude-md
stars: 16323
last_pushed: 2026-06-14T11:17:05Z
license: bsd-3-clause
score: 9
domains: [backend, database, distributed-systems]
tags: [strict-quality-control, testing-optimizations, architectural-context]
curated: 2026-06-15
curated_by: config-scout
---

# weaviate/weaviate — claude-md

**Why it's worth keeping:** The 'no bug is ever out of scope' rule prevents the agent from ignoring side effects; the testing section includes specific optimizations to prevent slow Docker rebuilds during E2E tests.

**Summary:** Provides strict behavioral mandates for bug fixing and highly detailed technical instructions for building, testing, and navigating a complex Go-based database architecture.

**Source credibility:** High; Weaviate is a major, highly-starred open-source project with active development.

**Recency:** Extremely current, with updates as recent as this month.

**Source:** [weaviate/weaviate/CLAUDE.md](https://github.com/weaviate/weaviate/blob/24163aff9ea6af1ca80a74e8ecf10f6a81ae689f/CLAUDE.md) · 16323★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Weaviate is an open-source, cloud-native vector database written in Go. It stores both objects and vectors, supporting semantic search, hybrid search (BM25 + vector), RAG, and reranking.

## No bug is ever out of scope

This is a production database. Data loss and silent failures are unacceptable, full stop. If you uncover or even *suspect* a bug — adjacent failure mode, race window, edge case in a related journey, anything — you MUST address it in the same change set. Acceptable outcomes:

1. **Reproduce and fix it.** Include a regression test that fails without the fix and passes with it.
2. **Reproduce it and commit a failing (red) test** that pins the bug, then escalate explicitly to the user. Never silently leave a known-bad code path with no test.

Unacceptable:

- "Out of scope." There is no out of scope for bugs in this codebase. If you find one, you own it until it's either fixed or pinned with a failing test.
- "Known issue, leaving for follow-up." Same rule — pin it with a failing test before you stop working on it.
- Fixing only the one specific reproduct
```

</details>
