---
name: garethrhughes__fragile__claude-template
source: https://github.com/garethrhughes/fragile/blob/8b49f664cd11831b0139c21c4260d0f71fb4d306/.opencode/skills/CLAUDE.md.template
repo: garethrhughes/fragile
kind: claude-md
stars: 5
last_pushed: 2026-06-16T02:40:18Z
license: mit
score: 9
domains: [software-engineering, devops, architecture]
tags: [template, tiered-rules, adr-workflow, structured-governance]
curated: 2026-06-16
curated_by: config-scout
---

# garethrhughes/fragile — claude-md

**Why it's worth keeping:** The layered approach prevents instruction bloat by delegating specific rules to stack-specific files and uses an ADR/Proposal workflow to maintain project governance.

**Summary:** A high-maturity template that establishes a tiered rule system (Core vs. Stack Overlay) and a formal architectural decision process.

**Source credibility:** Reflects professional engineering standards for structured documentation.

**Recency:** Highly current; utilizes modern 'skill' and 'profile' abstractions suited for agentic workflows.

**Source:** [garethrhughes/fragile/.opencode/skills/CLAUDE.md.template](https://github.com/garethrhughes/fragile/blob/8b49f664cd11831b0139c21c4260d0f71fb4d306/.opencode/skills/CLAUDE.md.template) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — [Project Name]

## Active Skillset: [typescript | dotnet | …]

This project follows the language-agnostic core rules in
[`.opencode/skills/RULES.md`](.opencode/skills/RULES.md) plus the matching stack
overlay in
[`.opencode/skills/rules/[profile].md`](.opencode/skills/rules/[profile].md)
(replace `[profile]` with the active skillset above — e.g. `typescript.md` or
`dotnet.md`).
Skills (`developer`, `reviewer`, `architect`, `infosec`) read both when applying
conventions to this project.

---

## Project Overview

[Short description: what does this system do, who uses it, what problem does it solve?]

---

## Tech Stack

### Backend
| Concern | Choice |
|---|---|
| Framework | [fill in] |
| Language | [fill in] |
| ORM / Data layer | [fill in] |
| Auth | [fill in] |
| API Docs | [fill in] |
| Testing | [fill in] |
| Migrations | [fill in] |
| Validation | [fill in — e.g. class-validator, Zod] |
| Logging | [fill in — e.g. pino, Winston] |

### Frontend
| Concern | Choice |
|---|---|
| Framework | [fill in] |
| Language | [fill in] |
| Styling | [fill in] |
| State | [fill in] |
| Testing | [fill in] |
| HTTP | [fill in] |
| Data fetching | [fill in — e.g. Server Compone
```

</details>
