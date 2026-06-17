---
name: piomin__claude-ai-spring-boot
source: https://github.com/piomin/claude-ai-spring-boot/blob/d87e7a38588a0a945ae2c11a251954897692330e/CLAUDE.md
repo: piomin/claude-ai-spring-boot
kind: claude-md
stars: 1217
last_pushed: 2026-04-29T07:02:03Z
license: apache-2.0
score: 8
domains: [backend-api, java, spring-boot]
tags: [agentic-workflow, self-improvement, engineering-standards]
curated: 2026-06-15
curated_by: config-scout
---

# piomin/claude-ai-spring-boot — claude-md

**Why it's worth keeping:** The 'Self-Improvement Loop' instruction (updating lessons.md) is a premier technique for long-term agentic context management, while the 'Verification Before Done' rule prevents common LLM hallucination errors.

**Summary:** Establishes a highly disciplined senior developer persona that prioritizes architectural elegance and systematic self-correction.

**Source credibility:** High; 1200+ stars and recent pushes suggest it is a well-vetted and maintained template.

**Recency:** Current; explicitly integrates modern Claude Code patterns like Plan Mode.

**Source:** [piomin/claude-ai-spring-boot/CLAUDE.md](https://github.com/piomin/claude-ai-spring-boot/blob/d87e7a38588a0a945ae2c11a251954897692330e/CLAUDE.md) · 1217★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
### 1. Plan Mode Default
- Enter plan mode for ANY not-trivial task (3+ steps or architectural decisions)
- Use plan mode for verification steps, not just building
- Write detailed specs upfront to reduce ambiguity

### 2. Self-Improvement Loop
- After ANY correction from the user: update `tasks/lessons.md` with the pattern
- Write rules for yourself that prevent the same mistake
- Ruthlessly iterate on these lessons until the mistake rate drops
- Review lessons at session start for a project

### 3. Verification Before Done
- Never mark a task complete without proving it works
- Diff behavior between main and your changes when relevant
- Ask yourself: "Would a staff engineer approve this?"
- Run tests, check logs, demonstrate correctness

### 4. Demand Elegance (Balanced)
- For non-trivial changes: pause and ask "is there a more elegant way?"
- If a fix feels hacky: "Knowing everything I know now, implement the elegant solution"
- Skip this for simple, obvious fixes. Don't overengineer
- Challenge your own work before presenting it

## Core Principles
- **Simplicity First**: Make every change as simple as possible. Impact minimal code
- **No Laziness**: Find root causes. No tempor
```

</details>
