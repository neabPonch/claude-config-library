---
name: shrek-abaper__sap-engineering-skill
source: https://github.com/shrek-abaper/sap-engineering-skill/blob/37d008cd1d9c87fe99a6db9a970c761212702489/CLAUDE.md
repo: shrek-abaper/sap-engineering-skill
kind: claude-md
stars: 20
last_pushed: 2026-05-29T01:56:17Z
license: mit
score: 9
domains: [agents-ai, cli-tools, sap-abap]
tags: [monorepo, tooling-orchestration, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# shrek-abaper/sap-engineering-skill — claude-md

**Why it's worth keeping:** It excels by documenting explicit command patterns, architectural hierarchy (how the Python logic is organized), and dependency maps that allow the agent to navigate complex toolsets without hallucination.

**Summary:** Provides highly structured operational guidance for an AI agent to interact with a suite of SAP engineering CLI tools and skill modules.

**Source credibility:** 20 stars; appears to be a specialized, high-utility repository for SAP automation.

**Recency:** Very recent; explicitly references current Claude Code/claude.ai capabilities.

**Source:** [shrek-abaper/sap-engineering-skill/CLAUDE.md](https://github.com/shrek-abaper/sap-engineering-skill/blob/37d008cd1d9c87fe99a6db9a970c761212702489/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Repository Overview

`sap-engineering-skill` is a monorepo of AI agent skills for SAP ABAP engineering. Each skill follows the `SKILL.md` specification and works with compatible AI agent frameworks (opencode, Claude Code, Cursor).

### Skills

| Skill | Purpose | Location |
|-------|---------|----------|
| `sap-adt-cli` | Read/write ABAP source and metadata via ADT REST API | `skills/sap-adt-cli/` |
| `abap-code-review` | Pre-release security & quality review (9 dimensions) | `skills/abap-code-review/` |
| `sap-transport-gate` | Transport Request release gate assessment (10 dimensions) | `skills/sap-transport-gate/` |
| `sap-integration-wiki` | SAP integration knowledge base (9 domains, 8 technologies) | `skills/sap-integration-wiki/` |

The three subtree skills (`abap-code-review`, `sap-transport-gate`, `sap-integration-wiki`) are maintained as independent public repositories and are tracked via git subtree remotes.

---

## Repository Structure

```
sap-engineering-skill/
├── skills/
│   ├── sap-adt-cli/              ← Source in this repo (main skill)
│   │
```

</details>
