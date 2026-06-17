---
name: KANG-Hyeong-uk__dcase_2026
source: https://github.com/KANG-Hyeong-uk/dcase_2026/blob/4a31c9374460cc5adb730d80c593daff62da91ee/skill.MD
repo: KANG-Hyeong-uk/dcase_2026
kind: skill
stars: 0
last_pushed: 2026-06-06T14:16:16Z
license: unknown
score: 9
domains: [backend-api, agents-ai, testing]
tags: [regression-testing, vitest, sandbox-mode, schema-validation]
curated: 2026-06-14
curated_by: config-scout
---

# KANG-Hyeong-uk/dcase_2026 — skill

**Why it's worth keeping:** Offers highly transferable Vitest patterns for API schema validation and defines a structured '/bug-check' command workflow that forces automated verification before AI review.

**Summary:** Establishes a regression testing framework specifically designed to combat 'AI blind spots' where models fail to notice inconsistencies between sandbox and production code paths.

**Source credibility:** Low star count, but contains high-signal, non-generic technical implementation details that suggest real-world utility.

**Recency:** Very current; addresses modern Next.js/Supabase stack and the specific failure modes of AI agents.

**Source:** [KANG-Hyeong-uk/dcase_2026/skill.MD](https://github.com/KANG-Hyeong-uk/dcase_2026/blob/4a31c9374460cc5adb730d80c593daff62da91ee/skill.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
name	ai-regression-testing
description	Regression testing strategies for AI-assisted development. Sandbox-mode API testing without database dependencies, automated bug-check workflows, and patterns to catch AI blind spots where the same model writes and reviews code.
origin	ECC
AI Regression Testing
Testing patterns specifically designed for AI-assisted development, where the same model writes code and reviews it — creating systematic blind spots that only automated tests can catch.

When to Activate
AI agent (Claude Code, Cursor, Codex) has modified API routes or backend logic
A bug was found and fixed — need to prevent re-introduction
Project has a sandbox/mock mode that can be leveraged for DB-free testing
Running /bug-check or similar review commands after code changes
Multiple code paths exist (sandbox vs production, feature flags, etc.)
The Core Problem
When an AI writes code and then reviews its own work, it carries the same assumptions into both steps. This creates a predictable failure pattern:

AI writes fix → AI reviews fix → AI says "looks correct" → Bug still exists
Real-world example (observed in production):

Fix 1: Added notification_settings to API response
  → For
```

</details>
