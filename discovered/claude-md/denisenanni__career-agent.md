---
name: denisenanni__career-agent
source: https://github.com/denisenanni/career-agent/blob/429ef8981636298b3ea97d4a0bc9804dc3f3778c/claude.md
repo: denisenanni/career-agent
kind: claude-md
stars: 0
last_pushed: 2025-12-27T18:52:18Z
license: mit
score: 7
domains: [backend-api, web-frontend, ai-agents]
tags: [safety-boundaries, workflow, fastapi, react]
curated: 2026-06-16
curated_by: config-scout
---

# denisenanni/career-agent — claude-md

**Why it's worth keeping:** The explicit 'Ask before' vs 'Never without asking' hierarchy is excellent for preventing destructive AI actions. It also provides high-value context on when to use specific model tiers (Haiku/Sonnet) for task execution.

**Summary:** Establishes a roadmap-driven workflow with clear state management and strict safety boundaries.

**Source credibility:** Low; based on a small personal repository with no social proof or description.

**Recency:** Current; the instructions are highly applicable to modern agentic workflows like Claude Code.

**Source:** [denisenanni/career-agent/claude.md](https://github.com/denisenanni/career-agent/blob/429ef8981636298b3ea97d4a0bc9804dc3f3778c/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Career Agent

**Stack:** Python FastAPI, React+TS+Vite, PostgreSQL, yarn

**Workflow:**
1. Check ROADMAP.md for current phase
2. Verify approach with me first
3. Complete tasks, mark [x] when done
4. Brief explanation of changes
5. Keep changes minimal

**Conventions:**
- Alembic migrations, pydantic validation
- Haiku=extraction, Sonnet=generation
- No 'any' - build types
- Check existing deps before installing

**Ask before:** migrations, deletes, new deps, .env/terraform edits, git push, destructive DB ops, sudo

**Never without asking:** rm -rf, git push --force, DROP TABLE/DATABASE, terraform destroy

**Quality:** Check security, no sensitive data in frontend, no vulnerabilities
```

</details>
