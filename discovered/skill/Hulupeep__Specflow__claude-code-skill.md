---
name: Hulupeep__Specflow__claude-code-skill
source: https://github.com/Hulupeep/Specflow/blob/00ba20cbb5628fbf782e977c5d30704eff0a6877/context/CLAUDE-CODE-SKILL.md
repo: Hulupeep/Specflow
kind: skill
stars: 24
last_pushed: 2026-06-12T14:13:27Z
license: mit
score: 9
domains: [cli-tools, software-architecture, devops, ai-agents]
tags: [contract-enforcement, architectural-guardrails, automated-testing, llm-drift-prevention]
curated: 2026-06-16
curated_by: config-scout
---

# Hulupeep/Specflow — skill

**Why it's worth keeping:** It transforms passive guidelines into active enforcement by generating specialized contract tests and shell hooks that fail builds when non-negotiable patterns are violated.

**Summary:** A framework for converting natural language architectural rules into automated testing suites (YAML + Regex/Playwright) to prevent LLM-induced code drift.

**Source credibility:** Solid niche repository with growing interest (24 stars) focused on the specific problem of agentic drift.

**Recency:** Highly current; designed specifically for the Claude Code CLI workflow, including slash commands and CLAUDE.md integration.

**Source:** [Hulupeep/Specflow/context/CLAUDE-CODE-SKILL.md](https://github.com/Hulupeep/Specflow/blob/00ba20cbb5628fbf782e977c5d30704eff0a6877/context/CLAUDE-CODE-SKILL.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Specflow Skill for Claude Code

Create a `/specflow` slash command that sets up contract enforcement for any project.

## Quick Setup

```bash
mkdir -p ~/.claude/skills
```

Create `~/.claude/skills/specflow.md` with the content below.

---

## The Skill (Copy This Entire File)

```markdown
# Specflow Skill

Set up architectural contracts that prevent drift. Self-contained - no external docs needed.

## Trigger

/specflow

## Instructions

When the user runs /specflow, follow this workflow:

### Step 1: Interview the User

Ask these questions (user answers in plain English):

**Architecture:**
> "What architectural rules should NEVER be broken?"
> (If you don't know, I'll suggest best practices for your tech stack)

**Features:**
> "What features exist and how should they behave?"

**Journeys:**
> "What user journeys must always work?"
> (I'll suggest obvious ones based on your features)

### Step 2: Generate REQ IDs

From user answers, create IDs:
- Architecture: `ARCH-001`, `ARCH-002`, etc.
- Auth: `AUTH-001`, `AUTH-002`, etc.
- Features: `FEAT-001`, `FEAT-002`, etc.
- Security: `SEC-001`, `SEC-002`, etc.
- Journeys: `J-CHECKOUT-001`, `J-AUTH-001`, etc.

Format: `[DOMAIN]-[NUMB
```

</details>
