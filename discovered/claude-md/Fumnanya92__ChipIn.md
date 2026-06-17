---
name: Fumnanya92__ChipIn
source: https://github.com/Fumnanya92/ChipIn/blob/ffa9c6742d5724b8d96c1eda24fe52532e777d66/Claude.md
repo: Fumnanya92/ChipIn
kind: claude-md
stars: 0
last_pushed: 2026-03-18T20:45:43Z
license: unknown
score: 7
domains: [agents-ai, software-engineering-workflow]
tags: [agentic-patterns, state-management, self-improvement]
curated: 2026-06-14
curated_by: config-scout
---

# Fumnanya92/ChipIn — claude-md

**Why it's worth keeping:** The 'Self-Improvement Loop' pattern—updating a lessons file after user corrections—is an excellent, transferable way to prevent repetitive mistakes in AI sessions.

**Summary:** This config establishes a structured agentic workflow using external state files (todo.md and lessons.md) to manage long-term context and error prevention.

**Source credibility:** Low; the repository has zero stars and unverified authorship.

**Recency:** Current; it utilizes modern agentic strategies like subagent orchestration and plan-mode defaults.

**Source:** [Fumnanya92/ChipIn/Claude.md](https://github.com/Fumnanya92/ChipIn/blob/ffa9c6742d5724b8d96c1eda24fe52532e777d66/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Sam Agent Guidelines

---

## Workflow Orchestration

### 1. Plan Mode Default

- Enter plan mode for ANY non-trivial task (3+ steps or architectural decisions)
- If something goes sideways, STOP and re-plan immediately — don't keep pushing
- Use plan mode for verification steps, not just building
- Write detailed specs upfront to reduce ambiguity

### 2. Subagent Strategy

- Use subagents liberally to keep main context window clean
- Offload research, exploration, and parallel analysis to subagents
- For complex problems, throw more compute at it via subagents
- One task per subagent for focused execution

### 3. Self-Improvement Loop

- After ANY correction from the user: update `tasks/lessons.md` with the pattern
- Write rules for yourself that prevent the same mistake
- Ruthlessly iterate on these lessons until mistake rate drops
- Review lessons at session start for relevant project

### 4. Verification Before Done

- Never mark a task complete without proving it works
- Diff behavior between main and your changes when relevant
- Ask yourself: "Would a staff engineer approve this?"
- Run tests, check logs, demonstrate correctness

### 5. Demand Elegance (Balanced
```

</details>
