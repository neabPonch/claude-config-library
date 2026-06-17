---
name: etewiah__property_web_builder
source: https://github.com/etewiah/property_web_builder/blob/d42c2c26da73023ed6a24c1652497fdf3f293e38/CLAUDE.md
repo: etewiah/property_web_builder
kind: claude-md
stars: 621
last_pushed: 2026-06-14T16:00:16Z
license: mit
score: 9
domains: [web-development, ruby-on-rails, qa-testing]
tags: [git-safety, tdd, regression-prevention, rails]
curated: 2026-06-15
curated_by: config-scout
---

# etewiah/property_web_builder — claude-md

**Why it's worth keeping:** The 'Analyze Gap -> Add Test -> Search for Similar' workflow is a masterclass in preventing AI-driven regressions. The strict Git staging instructions prevent the common agent error of committing unrelated local changes.

**Summary:** Implements rigorous git safety protocols and a mandatory three-step testing ritual to ensure bug fixes are permanent and verified.

**Source credibility:** High; 621 stars and recent activity indicate a popular, real-world production project.

**Recency:** Current; aligns with modern development workflows including Playwright and Rails asset management.

**Source:** [etewiah/property_web_builder/CLAUDE.md](https://github.com/etewiah/property_web_builder/blob/d42c2c26da73023ed6a24c1652497fdf3f293e38/CLAUDE.md) · 621★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions for PropertyWebBuilder

This file contains instructions for Claude Code instances working on this project.

## Critical Rules

> **🚨 STOP! BEFORE ANY GIT COMMIT 🚨**
>
> You MUST ask the user "Would you like me to commit these changes?" and wait for explicit confirmation BEFORE running `git commit`. This is NON-NEGOTIABLE. Never auto-commit.

### Git Commit Safety

**NEVER commit changes you did not make in this session.**

**ALWAYS ask for user confirmation before committing.** Do not commit automatically. Show the user:
1. The files that will be committed
2. The proposed commit message
3. Wait for explicit approval (e.g., "yes", "ok", "commit it") before running `git commit`

**If you commit without asking first, you have violated the most important rule in this file.**

Before committing:
1. Run `git status` to see ALL modified and untracked files
2. Identify which files YOU modified vs files that were already modified before your session
3. Only stage files YOU explicitly created or modified
4. If you see untracked files or modifications you didn't make, DO NOT add them

When staging files:
- Use specific file paths: `git add path/to/file.rb` instead o
```

</details>
