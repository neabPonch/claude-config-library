---
name: zencity__databricks-logs-reader__02-claude-skill
source: https://github.com/zencity/databricks-logs-reader/blob/3f2d9c5b83158eb0485a38cc7f83e904c425f2f5/spec/02-claude-skill.md
repo: zencity/databricks-logs-reader
kind: skill
stars: 2
last_pushed: 2026-04-17T20:55:47Z
license: mit
score: 9
domains: [cli-tools, data-engineering, devops]
tags: [databricks, spark, log-analysis, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# zencity/databricks-logs-reader — skill

**Why it's worth keeping:** Demonstrates the 'Progressive Disclosure' pattern (Level 1-3) and provides specific logic for mapping raw error patterns to root causes, which transforms a simple command into an expert analysis agent.

**Summary:** A highly structured skill that wraps a CLI tool into a domain-expert troubleshooting workflow for Databricks logs.

**Source credibility:** The source is niche/low star, but the documentation quality reflects professional-grade tool design.

**Recency:** 

**Source:** [zencity/databricks-logs-reader/spec/02-claude-skill.md](https://github.com/zencity/databricks-logs-reader/blob/3f2d9c5b83158eb0485a38cc7f83e904c425f2f5/spec/02-claude-skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Skill: `/dbr-logs`

A Claude Code skill that wraps `dbr-logs` so developers can fetch and analyze Databricks job logs directly from a Claude conversation, without remembering CLI flags or leaving their terminal.

**Prerequisite**: The `dbr-logs` CLI tool (see [01-cli-tool.md](01-cli-tool.md)) must be installed.

## Skill Category

**Workflow Automation** (Category 2 per Anthropic's skill guide) — a multi-step process that benefits from consistent methodology, using Bash tool execution to call the installed `dbr-logs` CLI.

## Skill Folder Structure

```
dbr-logs/
├── SKILL.md                      # Main skill file (instructions + frontmatter)
└── references/
    └── log-structure.md          # Log directory structure reference (from cli-tool spec)
```

## SKILL.md Frontmatter

```yaml
---
name: dbr-logs
description: Fetch, search, and analyze Databricks job logs. Use when user mentions "job logs", "databricks logs", "executor logs", "driver logs", "spark job failed", "check logs for", or asks to debug a Databricks job failure. Do NOT use for general Spark code questions or Databricks cluster configuration.
allowed-tools: Bash Read Grep
metadata:
  author: dbr-logs con
```

</details>
