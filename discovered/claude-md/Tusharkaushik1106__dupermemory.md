---
name: Tusharkaushik1106__dupermemory
source: https://github.com/Tusharkaushik1106/dupermemory/blob/aad6f4537be3ab5b44705fe65a241f273e9228c0/claude.md
repo: Tusharkaushik1106/dupermemory
kind: claude-md
stars: 3
last_pushed: 2026-04-11T08:41:38Z
license: unknown
score: 8
domains: [chrome-extension, web-frontend, javascript]
tags: [manifest-v3, dom-manipulation, guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# Tusharkaushik1106/dupermemory — claude-md

**Why it's worth keeping:** Contains high-value technical patterns for React-controlled inputs and provides excellent meta-rules against silent refactoring and speculative implementation.

**Summary:** A highly disciplined set of operational guardrails designed to prevent API hallucinations and scope creep in Chrome Extension development.

**Source credibility:** Small personal project with low star count but demonstrates high-quality, expert-level instruction writing.

**Recency:** Very current; pushed 2 months ago.

**Source:** [Tusharkaushik1106/dupermemory/claude.md](https://github.com/Tusharkaushik1106/dupermemory/blob/aad6f4537be3ab5b44705fe65a241f273e9228c0/claude.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Operational Rules — DuperMemory Development

These are the rules I follow when working on this project. They exist to prevent hallucinated code, unnecessary complexity, and scope creep.

---

## Core Rules

### 1. No invented APIs
I do not use browser APIs, Chrome extension APIs, or web platform features unless I have confirmed they exist. If I am unsure, I say so and we verify first.

### 2. No imaginary libraries
Every `import` or `require` must reference a real, published package. If I want to add a dependency, I name it explicitly and ask before adding it. For this project, the default is zero dependencies.

### 3. Every file must be runnable
I do not write skeleton code, placeholder functions, or `// TODO` stubs unless explicitly asked. If a file is created, it must do what it claims to do.

### 4. Ask instead of assuming
If requirements are ambiguous — selector behavior, injection timing, event handling — I ask before writing code. A wrong assumption costs more than a clarifying question.

### 5. No jumping ahead in phases
We implement Phase 1 before Phase 2. Phase 2 before Phase 3. I do not speculatively implement future phase features "while I'm in the file."

###
```

</details>
