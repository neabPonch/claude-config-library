---
name: ybarsotti__dotfiles__claude-tmpl
source: https://github.com/ybarsotti/dotfiles/blob/76c4b02142b12689838f02e2502cc763782d4416/dot_claude/CLAUDE.md.tmpl
repo: ybarsotti/dotfiles
kind: claude-md
stars: 0
last_pushed: 2026-05-27T14:09:16Z
license: unknown
score: 8
domains: [knowledge-management, cli-tools, personal-productivity]
tags: [obsidian, linear, tool-use, cli-integration]
curated: 2026-06-16
curated_by: config-scout
---

# ybarsotti/dotfiles — claude-md

**Why it's worth keeping:** Exemplifies how to document custom CLI tools by providing specific command variations, search strategies (semantic vs keyword), and explicit intent triggers.

**Summary:** Integrates a personalized knowledge base (Obsidian) and project management (Linear) via specialized CLI tools.

**Source credibility:** Low visibility/stars, but the technical sophistication of tool definitions suggests an advanced user-driven setup.

**Recency:** Current; follows modern patterns for agentic interaction with local environments via CLI.

**Source:** [ybarsotti/dotfiles/dot_claude/CLAUDE.md.tmpl](https://github.com/ybarsotti/dotfiles/blob/76c4b02142b12689838f02e2502cc763782d4416/dot_claude/CLAUDE.md.tmpl) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Global CLAUDE.md
{{- if eq .machine.purpose "personal" }}

## Project Management

We track our tickets and projects in Linear (https://linear.app), a project management tool.
We use the `lineark` CLI tool for communicating with Linear. Use your Bash tool to call the
`lineark` executable. Run `lineark usage` to see usage information.

## Personal Knowledge Base (qmd)

We use `qmd` as a local search engine for our Obsidian knowledge base. When the user asks about
topics they've studied, personal notes, technical concepts, or references from their knowledge base,
use the `qmd` CLI via Bash to search for relevant information before answering.

### Collections available:
- **technical-studies-db** — PostgreSQL internals (heap pages, MVCC, indexing, query optimization, WAL, locks)
- **technical-studies-courses** — Software architecture MBA (DevOps, SRE, Cloud, microservices, SOLID, CI/CD)
- **resources** — AI/ML, code snippets (React, Python), data engineering, database design, DevOps, security, Rust
- **career** — Interview prep, career development, management skills
- **career-archive** — Archived project PRDs and architecture docs

### How to search:
```bash
# Best results — hybrid
```

</details>
