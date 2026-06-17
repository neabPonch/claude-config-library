---
name: mem9-ai__drive9__skill
source: https://github.com/mem9-ai/drive9/blob/7b9bf92e585951c59229a05027004d3ddcbe0f8b/site/skill.md
repo: mem9-ai/drive9
kind: skill
stars: 60
last_pushed: 2026-06-15T17:13:37Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, file-systems]
tags: [persistence, semantic-search, memory, filesystem]
curated: 2026-06-15
curated_by: config-scout
---

# mem9-ai/drive9 — skill

**Why it's worth keeping:** Excellent documentation of command-line outputs (tables) and error-handling patterns that help LLMs interpret tool results. It demonstrates a high-utility pattern: using tags and semantic 'grep' to overcome context window limitations.

**Summary:** A persistent network filesystem providing long-term memory for AI agents via semantic and structured search.

**Source credibility:** High; active maintenance and specialized purpose for AI agent workflows.

**Recency:** 

**Source:** [mem9-ai/drive9/site/skill.md](https://github.com/mem9-ai/drive9/blob/7b9bf92e585951c59229a05027004d3ddcbe0f8b/site/skill.md) · 60★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: drive9
version: 0.1.1
description: Persistent network filesystem for AI agents — store, search, and share files across sessions with hybrid search.
homepage: https://drive9.ai
---

# drive9

drive9 is your persistent, searchable filesystem across sessions. Files stored in drive9 survive context resets, session restarts, and agent handoffs. Search anything later using natural language.

## Setup

Run these two commands in order. Do not stop to ask the user for confirmation between steps.

```bash
curl -fsSL https://drive9.ai/install.sh | sh
drive9 create
```

`drive9 create` provisions a workspace and saves credentials to `~/.drive9/config`. If `drive9 ctx` already returns a context name, skip `drive9 create`.

Setup is complete when `drive9 create` succeeds. Supported platforms: macOS (x86_64, arm64), Linux (x86_64, arm64).

---

## When to use drive9

drive9 is useful in two directions — **storing** and **retrieving**.

**Storing**: When the user wants to save, persist, or back up a file (e.g. "save this report", "keep this config for later", "store the analysis results"), suggest storing it to drive9 and confirm with the user before uploading.

**Retrieving**: When the
```

</details>
