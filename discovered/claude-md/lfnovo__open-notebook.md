---
name: lfnovo__open-notebook
source: https://github.com/lfnovo/open-notebook/blob/d39af076605171bc5ef51441e20e2842af6618e4/CLAUDE.md
repo: lfnovo/open-notebook
kind: claude-md
stars: 30726
last_pushed: 2026-06-13T12:16:12Z
license: mit
score: 9
domains: [ai-agents, fullstack]
tags: [architecture-diagrams, hierarchical-structure]
curated: 2026-06-15
curated_by: config-scout
---

# lfnovo/open-notebook — claude-md

**Why it's worth keeping:** Demonstrates the use of hierarchical CLAUDE.md files for sub-modules and includes a critical 'Quirks & Gotchas' section to preemptively prevent operational errors.

**Summary:** Provides a comprehensive multi-tier architectural blueprint including visual ASCII diagrams and detailed tech stack definitions.

**Source credibility:** High; highly starred (30k+) and actively maintained repository.

**Recency:** Very current, referencing modern stacks like Next.js 16 and React 19.

**Source:** [lfnovo/open-notebook/CLAUDE.md](https://github.com/lfnovo/open-notebook/blob/d39af076605171bc5ef51441e20e2842af6618e4/CLAUDE.md) · 30726★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Open Notebook - Root CLAUDE.md

This file provides architectural guidance for contributors working on Open Notebook at the project level.

## Project Overview

**Open Notebook** is an open-source, privacy-focused alternative to Google's Notebook LM. It's an AI-powered research assistant enabling users to upload multi-modal content (PDFs, audio, video, web pages), generate intelligent notes, search semantically, chat with AI models, and produce professional podcasts—all with complete control over data and choice of AI providers.

**Key Values**: Privacy-first, multi-provider AI support, fully self-hosted option, open-source transparency.

---

## Three-Tier Architecture

```
┌─────────────────────────────────────────────────────────┐
│              Frontend (React/Next.js)                    │
│              frontend/ @ port 3000                       │
├─────────────────────────────────────────────────────────┤
│ - Notebooks, sources, notes, chat, podcasts, search UI  │
│ - Zustand state management, TanStack Query (React Query)│
│ - Shadcn/ui component library with Tailwind CSS         │
└────────────────────────┬────────────────────────────────┘
                         │ HTTP R
```

</details>
