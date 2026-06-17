---
name: thevibeworks__claude-code-docs__long-running-claude
source: https://github.com/thevibeworks/claude-code-docs/blob/7ed14253bbdd17b3d465554be0d120e9abe9ae1c/content/blog/research/long-running-Claude.md
repo: thevibeworks/claude-code-docs
kind: claude-md
stars: 17
last_pushed: 2026-06-16T15:48:59Z
license: mit
score: 9
domains: [scientific-computing, agents-ai, engineering]
tags: [agentic-workflows, long-running-tasks, test-oracles, memory-management]
curated: 2026-06-16
curated_by: config-scout
---

# thevibeworks/claude-code-docs — claude-md

**Why it's worth keeping:** Introduces high-level agentic patterns: using 'failed approaches' in changelogs to prevent loops, utilizing reference implementations as 'test oracles', and enforcing git-based coordination for recovery.

**Summary:** Defines an autonomous workflow for complex scientific tasks where CLAUDE.md acts as a living project plan and CHANGELOG.md serves as long-term memory.

**Source credibility:** High; authored by an Anthropic researcher on a complex scientific implementation (clax).

**Recency:** Very current; explicitly addresses Claude Code and long-horizon agentic tasks.

**Source:** [thevibeworks/claude-code-docs/content/blog/research/long-running-Claude.md](https://github.com/thevibeworks/claude-code-docs/blob/7ed14253bbdd17b3d465554be0d120e9abe9ae1c/content/blog/research/long-running-Claude.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Title: Long-running Claude for scientific computing

URL Source: https://www.anthropic.com/research/long-running-Claude

Markdown Content:
_In this post, Siddharth Mishra-Sharma_, _a researcher on the Discovery team, explains how to apply multi-day agentic coding workflows—test oracles, persistent memory, and orchestration patterns—to scientific computing tasks even outside of one’s domain._

### **The premise**

Most scientists currently using AI agents work in a conversational loop, managing each step of the process on a tight leash. As models have become [significantly better at long-horizon tasks](https://metr.org/time-horizons/) over the last year or so, a new way of working emerged: rather than getting involved with every detail, we can specify the high-level objective and set a team of agents loose to work autonomously. This makes it possible to complete projects in mere hours that might otherwise take us days, weeks, or even months. Certain types of scientific tasks fit well within this model, e.g., reimplementing a numerical solver, converting legacy scientific software written in an old Fortran dialect to a modern language, and debugging a large codebase against a referen
```

</details>
