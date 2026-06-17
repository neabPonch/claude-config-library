---
name: rykugur__demiurge
source: https://github.com/rykugur/demiurge/blob/2bbfb94f361542c63ce0f425dab9dbf916d6cc06/CLAUDE.md
repo: rykugur/demiurge
kind: claude-md
stars: 0
last_pushed: 2026-04-03T02:13:02Z
license: unknown
score: 8
domains: [agents-ai, fullstack-web, devops]
tags: [bun, typescript, git-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# rykugur/demiurge — claude-md

**Why it's worth keeping:** It includes high-value 'gotchas' like Docker requirements for SQLite tests and specific worktree management instructions. The explicit git confirmation workflow is an excellent template for controlling agent side effects.

**Summary:** Establishes strict Git protocols for autonomous agent behavior and provides critical environmental context for Bun/SQLite development.

**Source credibility:** Low social proof (0 stars), but the extreme specificity suggests it is a highly functional, real-world project file.

**Recency:** Very current, utilizing modern stacks like Bun, Next.js 14, and OpenTofu.

**Source:** [rykugur/demiurge/CLAUDE.md](https://github.com/rykugur/demiurge/blob/2bbfb94f361542c63ce0f425dab9dbf916d6cc06/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Assistant Context

**Project:** Demiurge - Autonomous Orchestrator Agent System  
**User:** Known as "The Emperor"

---

## Workflow Requirements

### Git Operations Require Confirmation
**ALWAYS ask The Emperor before committing or pushing code.**
- Present the diff and commit message for approval
- Wait for explicit confirmation (e.g., "yes", "commit it", "push")
- Never commit/push without permission
- Exception: Emergency fixes may be committed with explanation

## Code Conventions

### Code Style
- Use TypeScript with strict mode
- Follow existing patterns in the codebase
- Write tests using `bun:test`
- Use Zod for validation
- Prefer explicit types over `any`

### Commit Messages
- `feat:` for new features
- `fix:` for bug fixes
- `test:` for test additions
- `docs:` for documentation
- `chore:` for maintenance

## Preferences

- Prefer explicit over implicit
- Test-driven development (TDD) for core modules
- Subagent-driven development for complex features
- Frequent small commits over large ones
- Documentation in code (JSDoc) and in `docs/`
- Sun Eater quotes in user-facing applications (flavorful but minimal)

## Important Notes

- **Worktrees:** Use `.work
```

</details>
