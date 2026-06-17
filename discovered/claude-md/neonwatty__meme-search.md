---
name: neonwatty__meme-search
source: https://github.com/neonwatty/meme-search/blob/876726c4419db3785e076ebc94a8cbc56f19d31a/CLAUDE.md
repo: neonwatty/meme-search
kind: claude-md
stars: 679
last_pushed: 2026-05-31T22:41:25Z
license: apache-2.0
score: 9
domains: [backend-api, microservices, testing-automation]
tags: [agentic-workflows, mocking-patterns, documentation-management, microservices]
curated: 2026-06-14
curated_by: config-scout
---

# neonwatty/meme-search — claude-md

**Why it's worth keeping:** The specialized 'Task Agent Usage Guidelines' teach the LLM how to use its own sub-agents effectively, while the distinction between temporary and permanent documentation prevents git clutter.

**Summary:** A highly advanced guide that manages complex microservices architecture by defining specific subagent behaviors and rigorous documentation storage rules. It provides actionable mocking patterns and environment setup via mise.

**Source credibility:** Strong; high star count (679) and very recent activity.

**Recency:** Current; leverages modern toolchains like mise and specific agentic workflows relevant to Claude Code.

**Source:** [neonwatty/meme-search/CLAUDE.md](https://github.com/neonwatty/meme-search/blob/876726c4419db3785e076ebc94a8cbc56f19d31a/CLAUDE.md) · 679★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 📁 File Organization Guidelines

**⚠️ IMPORTANT - Temporary Documentation Files**:
- **All temporary markdown files** created without explicit user request **MUST** be saved to `/plans/temp/`
- Examples: exploration notes, research summaries, draft documentation, intermediate analysis
- Permanent documentation (user-requested plans, design docs) goes in `/plans/`
- The `/plans/temp/` directory is git-ignored and not tracked in version control

## 🤖 Task Agent Usage Guidelines

**IMPORTANT**: Use specialized Task agents liberally for exploration, planning, and research tasks.

### When to Use Task Agents

**Explore Agent** (use `subagent_type=Explore`):
- Understanding codebase structure and architecture
- Finding where features are implemented across multiple files
- Exploring error handling patterns, API endpoints, or design patterns
- Questions like "How does X work?", "Where is Y handled?", "What's the structure of Z?"
- Set thoroughness: `quick` (basic), `medium` (moderate), or `very thorough` (comprehensive)

**Plan Agent** (use `subagent_type=Plan`):
- Breaki
```

</details>
