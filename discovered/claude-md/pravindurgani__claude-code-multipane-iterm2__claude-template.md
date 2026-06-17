---
name: pravindurgani__claude-code-multipane-iterm2__claude-template
source: https://github.com/pravindurgani/claude-code-multipane-iterm2/blob/c549e7bcba67adb8d04389f1788dd7e3551c5c7c/CLAUDE.md.template
repo: pravindurgani/claude-code-multipane-iterm2
kind: claude-md
stars: 3
last_pushed: 2026-06-06T10:56:46Z
license: mit
score: 8
domains: [cli-tools, developer-productivity, ai-agents]
tags: [template, meta-instructions, workflow-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# pravindurgani/claude-code-multipane-iterm2 — claude-md

**Why it's worth keeping:** It introduces elite patterns like 'Session Continuity' (enforcing state verification via git/logs) and a 'Lessons' section to create a formal feedback loop for preventing recurring mistakes.

**Summary:** A meta-template for global configuration (~/.claude/CLAUDE.md) that establishes user persona, technical guardrails, and session management.

**Source credibility:** Low star count (3 stars), but provides a highly specific, tactical workflow for CLI-based agent interaction.

**Recency:** Very current; it addresses the critical problems of context drift and state management inherent in modern tool-using agents.

**Source:** [pravindurgani/claude-code-multipane-iterm2/CLAUDE.md.template](https://github.com/pravindurgani/claude-code-multipane-iterm2/blob/c549e7bcba67adb8d04389f1788dd7e3551c5c7c/CLAUDE.md.template) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Global Rules
#
# INSTRUCTIONS:
#   1. Copy this file to ~/.claude/CLAUDE.md
#   2. Fill in or delete each section — keep only what you'll actually use
#   3. Do NOT commit this file; it is personal (project rules go in .claude/CLAUDE.md)
#
# Tip: Start with just the Identity and Active Constraints sections.
# Add more as your workflow matures. A 20-line file you read is better
# than a 200-line file you ignore.

---

## Identity

<!-- One sentence: your role and primary work context.
     Claude reads this at the start of every session.
     Example: "I am a backend engineer working primarily in Python and Go." -->

---

## Stack

<!-- Languages, frameworks, and tools you use regularly.
     Claude uses this to calibrate suggestions and code style.
     Example:
     - Python 3.12, pytest, Pydantic, FastAPI
     - TypeScript, React, Vite
     - Docker, GitHub Actions, Fly.io -->

---

## Active Constraints

<!-- Hard rules Claude must never violate.
     Be specific — vague rules are ignored.
     Examples:
     - Never push to main directly — always branch + PR.
     - Never edit .env files without my explicit confirmation.
     - Never install packages globally — us
```

</details>
