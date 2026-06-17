---
name: SynkraAI__aiox-squads__claude
source: https://github.com/SynkraAI/aiox-squads/blob/66118db856ef655b8cf5ba44eda963ad4d0b1d78/squads/apex/CLAUDE.md
repo: SynkraAI/aiox-squads
kind: claude-md
stars: 96
last_pushed: 2026-03-15T15:29:27Z
license: unknown
score: 9
domains: [web-frontend, agents-ai, orchestration]
tags: [multi-agent, persona-framework, frontend]
curated: 2026-06-15
curated_by: config-scout
---

# SynkraAI/aiox-squads — claude-md

**Why it's worth keeping:** The explicit agent delegation rules (orchestrator-to-specialist) and the 'intent clarification' bridge ensure high accuracy and user control before any code is changed.

**Summary:** Defines a sophisticated multi-agent orchestration system for frontend development, featuring specialized personas and rigorous handoff protocols.

**Source credibility:** Community-driven project with significant social proof via star count.

**Recency:** Very current; utilizes latest tech stacks like React 19 and Tailwind 4.

**Source:** [SynkraAI/aiox-squads/squads/apex/CLAUDE.md](https://github.com/SynkraAI/aiox-squads/blob/66118db856ef655b8cf5ba44eda963ad4d0b1d78/squads/apex/CLAUDE.md) · 96★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Apex Squad — Autonomous Frontend Intelligence

## Single Entry Point

**The user does not need to know commands or agent names.** Simply describe what you want in natural language.

```
@apex {any natural language description}
```

Apex automatically:
1. **Scans the project** (stack, structure, design patterns) via `apex-scan`
2. **Classifies the intent** (fix, improve, create, redesign, audit, question)
3. **Selects the pipeline** (*apex-fix, *apex-quick, *apex-go, or direct response)
4. **Routes to the right agents** (based on detected profile)
5. **Presents the plan** and waits for confirmation
6. **Executes and suggests improvements** after completion

### Natural usage examples

| User says | Apex does |
|-----------|-----------|
| "the header breaks on mobile viewports" | *apex-fix → @css-eng |
| "add entrance animation to the card" | *apex-fix → @motion-eng |
| "create a stats component with charts" | *apex-quick → @react-eng + @css-eng |
| "redesign the entire services page" | *apex-go → full pipeline |
| "how's the accessibility?" | *apex-audit (no pipeline) |
| "which components use motion?" | Direct response (no pipeline) |
| "extract colors from linear.app" | *scrape
```

</details>
