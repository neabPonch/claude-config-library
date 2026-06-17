---
name: MervinPraison__PraisonAI__trigger-claude
source: https://github.com/MervinPraison/PraisonAI/blob/1ad58ca02975ff1398efeda694ea2ab78f20cf3e/src/praisonai-agents/.agent/workflows/trigger-claude.md
repo: MervinPraison/PraisonAI
kind: claude-md
stars: 8138
last_pushed: 2026-06-15T09:47:41Z
license: mit
score: 9
domains: [agents-ai, cli-tools, python]
tags: [architecture-rules, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# MervinPraison/PraisonAI — claude-md

**Why it's worth keeping:** Implements mandatory 'Architecture Validation' steps to force reasoning; provides specific file-path and inheritance rules to prevent technical debt.

**Summary:** A rigorous execution workflow that enforces strict architectural routing (Core vs. Wrapper) and code-size constraints before implementation begins.

**Source credibility:** High; the repository is highly starred and actively maintained.

**Recency:** Current; designed for modern agentic workflows using GitHub CLI integration.

**Source:** [MervinPraison/PraisonAI/src/praisonai-agents/.agent/workflows/trigger-claude.md](https://github.com/MervinPraison/PraisonAI/blob/1ad58ca02975ff1398efeda694ea2ab78f20cf3e/src/praisonai-agents/.agent/workflows/trigger-claude.md) · 8138★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Trigger Claude to fix an issue using the full architectural prompt
---

Use this workflow when you want to manually trigger Claude on an issue (especially for external users) using the complete, strict set of architectural rules. 

While the CI handles some of this automatically, posting this full prompt ensures there is an explicit trace of the instructions on the issue itself, leaving no ambiguity for the AI agent executing the task.

### 1. View Recent External Issues

```bash
// turbo
gh issue list --state open --limit 10
```

### 2. Post the Full @claude Trigger Prompt

Replace `<ISSUE_NUMBER>` with the target issue and run:

```bash
ISSUE_NUMBER="<ISSUE_NUMBER>"

PROMPT=$(cat << 'EOF'
@claude
You are working on the PraisonAI SDK. Follow AGENTS.md strictly.

STEP 0 — SETUP GIT IDENTITY:
git config user.name "MervinPraison"
git config user.email "454862+MervinPraison@users.noreply.github.com"

STEP 1 — READ GUIDELINES:
Read AGENTS.md to understand the architecture rules.

STEP 2 — ARCHITECTURE VALIDATION & ROUTING (MANDATORY before writing code):
Before implementing anything, answer these questions:
- CORE vs WRAPPER vs TOOLS ROUTING:
  1. Core SDK (praisonaiag
```

</details>
