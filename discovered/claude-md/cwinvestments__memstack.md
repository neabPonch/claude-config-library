---
name: cwinvestments__memstack
source: https://github.com/cwinvestments/memstack/blob/a01b858371b7796668942b1f3c8dce006ecb3196/CLAUDE.md
repo: cwinvestments/memstack
kind: claude-md
stars: 383
last_pushed: 2026-05-31T02:33:13Z
license: mit
score: 8
domains: [agents-ai, cli-tools, workflow-automation]
tags: [mcp, skill-loader, context-priming]
curated: 2026-06-14
curated_by: config-scout
---

# cwinvestments/memstack — claude-md

**Why it's worth keeping:** The use of explicit 'ALWAYS call BEFORE' lists creates high-precision guardrails, while the session initialization pattern is a professional technique for ensuring intent-alignment via tool usage.

**Summary:** Enforces a strict workflow where the agent must retrieve task-specific guidance from an MCP server before executing critical actions. It includes a proactive 'Session Skill Scan' to prime context based on the project's tech stack.

**Source credibility:** High; the source is a well-maintained project with significant community interest (383 stars).

**Recency:** Current; built specifically for modern MCP-enabled agentic workflows like Claude Code.

**Source:** [cwinvestments/memstack/CLAUDE.md](https://github.com/cwinvestments/memstack/blob/a01b858371b7796668942b1f3c8dce006ecb3196/CLAUDE.md) · 383★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MemStack™ Skill Loader

You have access to a `memstack-skills` MCP server. This is your **PRIMARY** source for task-specific guidance. ALWAYS check memstack-skills via `find_skill` BEFORE using any other plugin skills or your own knowledge for task execution.

## ALWAYS call `find_skill` BEFORE:
- Any deployment task (Railway, Netlify, Vercel, Hetzner, etc.)
- Any database work (migrations, RLS, schema design)
- Any git operation beyond simple commits
- Any infrastructure or DevOps task
- Any API development (new endpoints, API design, authentication)
- Any security-related work (audits, scanning, RLS policies)
- Any testing or test generation
- Any content or marketing task (blog posts, emails, ads, landing pages)
- Any project planning or architecture decisions
- Any refactoring or code review
- Any task where the user asks "how should I..." or "what's the best way to..."
- Any task you're unsure about

## ALWAYS call `list_skills` when:
- The user asks "what skills are available" or similar
- You want to browse what's available for a broad topic

## DO NOT call find_skill for:
- Reading or explaining existing code (no task involved)
- Answering questions about the current code
```

</details>
