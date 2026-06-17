---
name: sruja-ai__sruja__getting-started-skill
source: https://github.com/sruja-ai/sruja/blob/d495b49f8bdbd417ef2993adcaefbb7d3f98f0b7/docs/GETTING_STARTED_SKILL.md
repo: sruja-ai/sruja
kind: skill
stars: 22
last_pushed: 2026-06-15T06:16:06Z
license: apache-2.0
score: 8
domains: [cli-tools, architecture-as-code, agents-ai, devops]
tags: [architecture, guardrails, verification, drift-detection]
curated: 2026-06-16
curated_by: config-scout
---

# sruja-ai/sruja — skill

**Why it's worth keeping:** The use of 'verify-task' as a completion gate and the 'impact' command for blast radius estimation are elite patterns for maintaining large codebases with AI. It shifts from conversational prompting to validating architectural integrity against structured evidence.

**Summary:** A structural intelligence framework that uses a machine-readable 'repo.sruja' file to manage architectural drift and enforce task verification. It introduces high-leverage commands for impact analysis and automated linting of code structure.

**Source credibility:** Small, focused toolset (22 stars) with high-quality documentation and active maintenance.

**Recency:** Very current; aligns perfectly with modern MCP-driven agentic workflows.

**Source:** [sruja-ai/sruja/docs/GETTING_STARTED_SKILL.md](https://github.com/sruja-ai/sruja/blob/d495b49f8bdbd417ef2993adcaefbb7d3f98f0b7/docs/GETTING_STARTED_SKILL.md) · 22★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Getting Started with Sruja Skills

**AI coding harness + optional architecture authoring.**

Sruja is not a second coding agent. Install the **harness** skill so any agent runs `verify-task` before done; add **sruja-architecture** when you want reviewed `repo.sruja` in Git.

See [INSTALL_AS_SKILL.md](INSTALL_AS_SKILL.md) and [COMMUNITY_SKILLS_STACK.md](COMMUNITY_SKILLS_STACK.md).

---

## What You'll Need

1. **Sruja CLI** – Scan, drift, focus, verify-task
2. **AI editor** – Cursor, Copilot, Claude, etc. (owns the LLM loop)
3. **Skills** – `sruja-harness` (required for gates); `sruja-architecture` (optional)

---

## Tier 1 workflow (harness)

```
focus / drift  →  host agent edits code  →  verify-task  →  (optional) agent record on failure
```

No `repo.sruja` required for structural scan and verify gates.

---

## Tier 1b workflow (architecture skill)

```
You → Tell AI to analyze your code
  ↓
AI → Runs discover / sync evidence
  ↓
AI → Generates repo.sruja
  ↓
AI → lint + drift against repo.sruja
```

---

## Quick Start (Copy These Steps)

### Step 1: Install CLI + harness skill

```bash
curl -fsSL https://sruja.ai/install.sh | bash
npx skills add https://github.com/sruja-ai
```

</details>
