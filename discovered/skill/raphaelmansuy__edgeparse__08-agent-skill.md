---
name: raphaelmansuy__edgeparse__08-agent-skill
source: https://github.com/raphaelmansuy/edgeparse/blob/98e2fa0132629078d07c19bfc8a8776fee85d8dd/docs/08-agent-skill.md
repo: raphaelmansuy/edgeparse
kind: skill
stars: 118
last_pushed: 2026-04-14T00:19:37Z
license: other
score: 9
domains: [agents-ai, data-extraction, cli-tools]
tags: [pdf-parsing, context-management, structured-data]
curated: 2026-06-15
curated_by: config-scout
---

# raphaelmansuy/edgeparse — skill

**Why it's worth keeping:** Implements a sophisticated three-level loading pattern (Description -> Core -> On-demand Reference) to optimize context window usage. It provides explicit decision heuristics for format selection and edge-case handling.

**Summary:** Teaches Claude how to use the EdgeParse library to convert PDFs into structured formats like Markdown and JSON.

**Source credibility:** High; well-maintained repository with significant community interest (118 stars).

**Recency:** Highly current, incorporating modern MCP integration patterns.

**Source:** [raphaelmansuy/edgeparse/docs/08-agent-skill.md](https://github.com/raphaelmansuy/edgeparse/blob/98e2fa0132629078d07c19bfc8a8776fee85d8dd/docs/08-agent-skill.md) · 118★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 08 — EdgeParse Agent Skill

EdgeParse ships as a **Claude agent skill** — a single installable unit that teaches Claude how to extract structured content from PDFs on behalf of users and autonomous agents.

Install once via `npx skills add`, and every Claude agent session in your project gains the ability to read, parse, and reason about PDF documents.

---

## What is a skill?

A skill is a structured Markdown file (`SKILL.md`) your AI agent pre-loads to gain domain-specific knowledge and tool-use patterns. The `npx skills add` command fetches the skill from GitHub and registers it in your project's `skills-lock.json`.

When Claude sees a PDF-related task, it reads the EdgeParse skill and knows:
- How to install and call `edgeparse.convert()`
- Which output format to use for different tasks (Markdown for LLMs, JSON for bounding boxes)
- How to handle tables, multi-column layouts, and encrypted files
- Recommended patterns for RAG pipelines, agent tools, and MCP servers

---

## Install

### Via `npx skills add` (recommended)

```bash
npx skills add raphaelmansuy/edgeparse --skill edgeparse
```

This adds an entry to your project's `skills-lock.json`:

```json
{
  "version": 1,
```

</details>
