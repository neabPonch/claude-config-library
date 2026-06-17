---
name: MrMoshkovitz__gm-claude__claude
source: https://github.com/MrMoshkovitz/gm-claude/blob/c3f8c2958f1e4e81dcdaa4df2c899e2cfe46ff9e/agentic-confs/LLM-Red-Team-Paylopads/CLAUDE.md
repo: MrMoshkovitz/gm-claude
kind: claude-md
stars: 0
last_pushed: 2026-01-03T11:14:01Z
license: unknown
score: 9
domains: [security, agents-ai, red-teaming]
tags: [agent-orchestration, safety-guardrails, mcp-integration]
curated: 2026-06-14
curated_by: config-scout
---

# MrMoshkovitz/gm-claude — claude-md

**Why it's worth keeping:** The 'Specialized Subagents' section is a premier template for defining proactive roles, triggers, and MCP dependencies. The inclusion of permission schemas and shell-based safety hooks demonstrates an advanced pattern for high-security agentic environments.

**Summary:** This config acts as a sophisticated orchestration guide that defines specialized subagents with specific triggers, purposes, and toolsets. It provides high-level instructions for managing an AI-driven red-teaming workflow.

**Source credibility:** Low social proof (0 stars) but the technical density suggests highly specialized expertise in AI security.

**Recency:** Very current; utilizes modern agent-orchestration patterns and MCP server integration.

**Source:** [MrMoshkovitz/gm-claude/agentic-confs/LLM-Red-Team-Paylopads/CLAUDE.md](https://github.com/MrMoshkovitz/gm-claude/blob/c3f8c2958f1e4e81dcdaa4df2c899e2cfe46ff9e/agentic-confs/LLM-Red-Team-Paylopads/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# LLM Red Team Payloads - Claude Code Configuration

## Project Overview
This repository contains OWASP AI Testing Guide (AITG) payloads for defensive AI security research. The project provides sanitized red team scenarios, test datasets, and evaluation frameworks for assessing LLM security vulnerabilities in authorized testing environments.

### Tech Stack
- **Languages**: YAML (test configurations), Python (analysis scripts), JSON (results)
- **Frameworks**: OWASP AITG, MITRE ATLAS
- **Models Tested**: GPT-5, Gemini 2.5 Flash, Claude Sonnet 4, Llama 4 Maverick
- **Data Formats**: CSV (results), JSONL (detailed logs), YAML (test configs)

### Entry Points
- **AITG Test Files**: `OWASP AITG-APP/AITG-APP-*.yaml` (14 test categories)
- **Results Analysis**: `OWASP AITG-APP/RESULTS/` (model performance data)
- **Dataset Generation**: `CSVs/` (training datasets for ML)

### Run/Test Commands
```bash
# Validate YAML structure
python3 -c \"import yaml; yaml.safe_load(open('OWASP AITG-APP/AITG-APP-01.yaml'))\"

# Basic results analysis
head -5 \"OWASP AITG-APP/RESULTS/anthropic-claude-sonnet-4-results.csv\"

# Safety compliance check
grep -r \"<SECRET>\\|<REDACTED>\" --include=\"*.yaml\"
```

</details>
