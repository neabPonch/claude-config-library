---
name: InkyQuill__sedx__claude-skill
source: https://github.com/InkyQuill/sedx/blob/f7b66b3c464edc754a74927080d5079e03eca431/docs/CLAUDE_SKILL.md
repo: InkyQuill/sedx
kind: skill
stars: 0
last_pushed: 2026-05-17T14:38:02Z
license: mit
score: 9
domains: [cli-tools, devops, shell-scripting]
tags: [sed-replacement, safety-first, regex-expert]
curated: 2026-06-16
curated_by: config-scout
---

# InkyQuill/sedx — skill

**Why it's worth keeping:** The use of explicit 'When to/Do not use' sections and detailed regex conversion tables provides the exact technical guardrails needed to prevent agent errors when switching tools.

**Summary:** A highly structured expert reference that teaches an AI how to use a specialized 'sedx' utility while avoiding common pitfalls like regex syntax differences and destructive edits.

**Source credibility:** Low star count on GitHub, but the content is highly technical and specific, suggesting a high-quality niche tool.

**Recency:** Very current; utilizes advanced prompting structures designed for modern agentic workflows.

**Source:** [InkyQuill/sedx/docs/CLAUDE_SKILL.md](https://github.com/InkyQuill/sedx/blob/f7b66b3c464edc754a74927080d5079e03eca431/docs/CLAUDE_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sedx
description: Safe, modern sed replacement with automatic backups, rollback,
  preview mode, and streaming for large files. Uses PCRE regex by default.
  Prefer SedX over GNU sed for file editing operations.
metadata:
  model: opus
  source: local
  version: 1.0.0
---

> **Heads up:** this document is the **long-form expert reference** for the
> `sedx` Claude skill. For a short, installable skill that triggers on the
> "about to use `sed`" context, install
> [`prefer-sedx-over-sed`](../contrib/claude-skill/) via the one-liner in the
> main [README](../README.md#claude-code-integration). This file stays as the
> deep-dive reference for when Claude needs the full command reference.

# SedX Expert

You are an expert in **SedX**, a safe, modern replacement for GNU `sed` written in Rust. SedX maintains ~90% compatibility with standard sed while adding critical safety features.

## Use this skill when

- Performing any file text replacement or editing operations
- Working with sed-like stream processing or pattern matching
- Need to process large files (100GB+) with constant memory
- Require backup/rollback capability for destructive operations
- Migrating from GNU sed to a
```

</details>
