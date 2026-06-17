---
name: hilash__cabinet__claude
source: https://github.com/hilash/cabinet/blob/9ba42f65b21b9dbcf2679d9e051bab1dd6197d4b/docs/CLAUDE.md
repo: hilash/cabinet
kind: claude-md
stars: 2276
last_pushed: 2026-06-15T08:23:12Z
license: mit
score: 9
domains: [full-stack, ai-agents, knowledge-management]
tags: [architecture-map, rules-engine, system-spec]
curated: 2026-06-15
curated_by: config-scout
---

# hilash/cabinet — claude-md

**Why it's worth keeping:** It utilizes explicit directory mappings to explain system intent and enforces highly granular rules (e.g., path traversal prevention, component usage nuances) that prevent common agent errors. The inclusion of specific stylistic constraints like the 'em-dash rule' is an expert touch for maintaining brand voice.

**Summary:** This file provides a comprehensive structural and operational blueprint for a complex AI-first platform. It moves beyond simple commands to provide a deep mental model of the project's architecture.

**Source credibility:** High; from a prominent, actively maintained repository with significant community interest.

**Recency:** Very current; reflects modern full-stack and AI-orchestration workflows.

**Source:** [hilash/cabinet/docs/CLAUDE.md](https://github.com/hilash/cabinet/blob/9ba42f65b21b9dbcf2679d9e051bab1dd6197d4b/docs/CLAUDE.md) · 2276★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Cabinet

## What is this project?

Cabinet is an AI-first self-hosted knowledge base and startup OS. All content lives as markdown files on disk. The web UI provides WYSIWYG editing, a collapsible tree sidebar, drag-and-drop page organization, structured AI runs for tasks/jobs/heartbeats, and interactive `WebTerminal` surfaces for direct CLI sessions.

**Core philosophy:** Humans define intent. Agents do the work. The knowledge base is the shared memory between both.

## Tech Stack

- **Framework:** Next.js 16 (App Router), TypeScript
- **UI:** Tailwind CSS + shadcn/ui (base-ui based, NOT Radix — no `asChild` prop)
- **Editor:** Tiptap (ProseMirror-based) with markdown roundtrip via HTML intermediate
- **State:** Zustand (tree-store, editor-store, ai-panel-store, task-store, app-store)
- **Fonts:** Inter (sans) + JetBrains Mono (code)
- **Icons:** Lucide (no emoji in system chrome)
- **Markdown:** gray-matter (frontmatter), unified/remark (MD→HTML), turndown (HTML→MD)
- **AI providers:** Claude Code, Codex CLI, Cursor CLI, OpenCode, Copilot CLI, Grok CLI, Pi, and a generic CLI adapter — all driven through the shared adapter runtime in `src/lib/agents/`.

## Architectu
```

</details>
