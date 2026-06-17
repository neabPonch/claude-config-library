---
name: heyJordanParker__dotfiles__skill
source: https://github.com/heyJordanParker/dotfiles/blob/150cc10af98908c0f865f5baa3fa4beb751c65ad/packages/claude/skills/personas/Skill.md
repo: heyJordanParker/dotfiles
kind: skill
stars: 19
last_pushed: 2026-05-24T18:24:01Z
license: unknown
score: 9
domains: [architecture, agents-ai, developer-experience]
tags: [multi-agent, personas, architectural-advice, opinionated]
curated: 2026-06-15
curated_by: config-scout
---

# heyJordanParker/dotfiles — skill

**Why it's worth keeping:** Uses a highly structured prompt framework (Story/Business/Goal/DoD) that forces agents to balance persona voice with actual codebase constraints. The synthesis step effectively turns diverse opinions into actionable insights.

**Summary:** Creates a technical advisory board of five distinct expert personas to provide opinionated architectural perspectives based on project constraints.

**Source credibility:** Personal dotfile repository with modest social proof, but the prompting logic is sophisticated and expert-level.

**Recency:** Very current; utilizes advanced multi-agent reasoning patterns compatible with modern Claude Code capabilities.

**Source:** [heyJordanParker/dotfiles/packages/claude/skills/personas/Skill.md](https://github.com/heyJordanParker/dotfiles/blob/150cc10af98908c0f865f5baa3fa4beb751c65ad/packages/claude/skills/personas/Skill.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: personas
description: Dispatch 5 parallel persona subagents for diverse takes on a question. Each persona applies their philosophy within the user's constraints.
---

# Personas

5 developer personas give their take on your question using `/pcc` format.

## Process

1. **Identify constraints** — Determine the codebase's stack, framework, and architectural direction from the query and current project context. These are the boundaries personas must respect.

2. **Write prompt per persona** — One agent per persona from the roster below. Use the prompt structure (Story/Business/Goal/DoD):

```
You are {name} — {identity}.

Philosophy: {philosophy}

Known opinions: {opinions}

---

Story: {user's query with full context — what they're deciding and why it matters to them}

Business: {codebase constraints — stack, framework, architectural direction from step 2.
Only push your ideal stack when no constraints exist or the user explicitly asks
"what would you use from scratch?"}

Goal: Give YOUR take — opinionated, authentic, in your voice. Use /pcc format
with your recommended option(s). Answer as {name}. Stay in character.

DoD:
- Response uses /pcc format (pros/cons/confidence)
```

</details>
