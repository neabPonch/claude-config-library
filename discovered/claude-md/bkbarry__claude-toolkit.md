---
name: bkbarry__claude-toolkit
source: https://github.com/bkbarry/claude-toolkit/blob/fca6f7557e50cb93813dbf8e47e49099378aa1dd/claude.md
repo: bkbarry/claude-toolkit
kind: claude-md
stars: 0
last_pushed: 2026-03-31T16:16:54Z
license: unknown
score: 8
domains: [general-software-engineering, workflow-optimization]
tags: [philosophy, knowledge-management, communication-protocol]
curated: 2026-06-14
curated_by: config-scout
---

# bkbarry/claude-toolkit — claude-md

**Why it's worth keeping:** The 'analog-driven implementation' instruction prevents pattern drift, while the manual knowledge base workflow solves the problem of ephemeral AI context.

**Summary:** Establishes strict architectural principles and a noise-reducing communication protocol. It introduces an externalized memory pattern via 'kb/' and 'learnings' files to persist context between sessions.

**Source credibility:** Low social proof (0 stars), but content reflects high architectural maturity.

**Recency:** Highly relevant to modern agentic workflows and long-term context management.

**Source:** [bkbarry/claude-toolkit/claude.md](https://github.com/bkbarry/claude-toolkit/blob/fca6f7557e50cb93813dbf8e47e49099378aa1dd/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# How I Work

## Philosophy
- Plan before code. For anything non-trivial, understand the problem and plan the approach before writing.
- Analog-driven implementation. Before building something new, find existing code that does something similar and follow its patterns exactly.
- Human-in-the-loop for hard decisions. Data models, state machines, system boundaries — stop and ask rather than guessing.
- Ship incrementally. Prefer small, independently mergeable changes over big bangs.

## Code Style
- Functions over classes. Classes are for data modeling only (Pydantic, dataclasses, ORM models).
- Fail loudly. No silent error swallowing, no catch-and-ignore, no bare except clauses.
- Validate at boundaries, trust data inside. Don't re-validate what the schema already enforces.
- No over-engineering. Don't add abstractions for one-time operations. Three similar lines > premature abstraction.
- One file first. Split when it's actually big (~300+ lines with clear seams), not preemptively.
- No optional arguments without a good reason. The default is things aren't optional.

## Communication
- Be concise. Bullets over paragraphs.
- Don't summarize what you just did — I can read the diff.
-
```

</details>
