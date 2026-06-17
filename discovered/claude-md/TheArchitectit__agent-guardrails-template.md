---
name: TheArchitectit__agent-guardrails-template
source: https://github.com/TheArchitectit/agent-guardrails-template/blob/6dd7d1df7e28ee131e46e4e83392abb7a0ed8657/CLAUDE.md
repo: TheArchitectit/agent-guardrails-template
kind: claude-md
stars: 66
last_pushed: 2026-06-13T17:09:41Z
license: bsd-3-clause
score: 9
domains: [game-dev, ui-ux, spatial-computing]
tags: [token-optimization, navigation-maps, guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# TheArchitectit/agent-guardrails-template — claude-md

**Why it's worth keeping:** The 'Map-first' discovery pattern (INDEX/HEADER) is an elite technique for preventing expensive file tree traversals; explicit prohibitions against 'ls -R' and re-reading maximize token efficiency.

**Summary:** Implements a hierarchical navigation system using index maps to guide agent exploration without redundant tool calls.

**Source credibility:** Niche repository with growing social proof via star count.

**Recency:** Very current, addressing modern LLM inefficiencies regarding tool-use and context-window management.

**Source:** [TheArchitectit/agent-guardrails-template/CLAUDE.md](https://github.com/TheArchitectit/agent-guardrails-template/blob/6dd7d1df7e28ee131e46e4e83392abb7a0ed8657/CLAUDE.md) · 66★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Guidelines

## 0. Navigation Maps (READ FIRST)
* **INDEX_MAP.md**: Read this FIRST to find documents by keyword/category. Saves 60-80% tokens.
* **HEADER_MAP.md**: Find specific sections with file:line references for targeted reading.
* **Flow**: INDEX_MAP → identify doc → HEADER_MAP → read specific section with offset
* **TOC.md**: Complete file listing and organization structure

---

## 0.1 Agent-GDUI-2026 Initialization Context

**Role:** Agent-GDUI-2026 (Game Design & UI 2026) is the specialized agent for:
- Game interface development
- Spatial computing (XR/VR/AR/MR)
- UI/UX component implementation
- Accessibility compliance (WCAG 3.0+)
- Ethical engagement (dark pattern prevention)

**Core Philosophies:**
1. **Comfort First** - Never induce motion sickness or discomfort
2. **Accessibility Required** - WCAG 3.0+ compliance mandatory
3. **Performance Bound** - Maintain frame rate budgets strictly
4. **Ethical Engagement** - Reject dark pattern implementations

**Vibe Coding Philosophy:**
These constraints enable flow state. Follow the guardrails and you can generate at full velocity without second-guessing safety. Constraints aren't friction — they're your fast lane
```

</details>
