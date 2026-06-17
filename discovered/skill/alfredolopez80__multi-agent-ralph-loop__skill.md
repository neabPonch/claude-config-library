---
name: alfredolopez80__multi-agent-ralph-loop__skill
source: https://github.com/alfredolopez80/multi-agent-ralph-loop/blob/0ad994fdae563aa71f6d375fbcbd6c2d08b4adce/.claude/skills/defense-profiler/skill.md
repo: alfredolopez80/multi-agent-ralph-loop
kind: skill
stars: 138
last_pushed: 2026-06-14T15:21:20Z
license: other
score: 8
domains: [security, devsecops, backend-api]
tags: [profiling, security-audit, schema-driven]
curated: 2026-06-15
curated_by: config-scout
---

# alfredolopez80/multi-agent-ralph-loop — skill

**Why it's worth keeping:** The predefined 'Analysis Dimensions' and the rigorous `DefenseProfile` schema transform vague security observations into a disciplined, multi-layered auditing process worth adopting for any security agent.

**Summary:** A highly structured security profiling system that uses specific analysis dimensions to build a mental model of a codebase's defensive capabilities.

**Source credibility:** High: The source repository is active, recently updated, and shows significant community traction via stars.

**Recency:** Current; designed to be model-agnostic and compatible with modern CLI-driven agentic workflows.

**Source:** [alfredolopez80/multi-agent-ralph-loop/.claude/skills/defense-profiler/skill.md](https://github.com/alfredolopez80/multi-agent-ralph-loop/blob/0ad994fdae563aa71f6d375fbcbd6c2d08b4adce/.claude/skills/defense-profiler/skill.md) · 138★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
# VERSION: 2.88.0
name: defense-profiler
description: "Codebase defense analysis system for security profiling"
user-invocable: true
---

# Defense Profiler

## v2.88 Key Changes (MODEL-AGNOSTIC)

- **Model-agnostic**: Uses model configured in `~/.claude/settings.json` or CLI/env vars
- **No flags required**: Works with the configured default model
- **Flexible**: Works with GLM-5, Claude, Minimax, or any configured model
- **Settings-driven**: Model selection via `ANTHROPIC_DEFAULT_*_MODEL` env vars

**Codebase Defense Analysis System** inspired by ZeroLeaks defense profiling.

Systematically analyzes code to build a comprehensive profile of security defenses, patterns, and weaknesses.

## Core Concept

Before attacking (testing), understand the defenses. Build a mental model of:
- What patterns exist
- What safeguards are in place
- What triggers failures
- What areas are weak

## Usage

```bash
/defense-profile src/
/defense-profile --focus security src/auth/
/defense-profile --output profile.json src/api/
```

## Defense Levels

| Level | Description | Characteristics |
|-------|-------------|-----------------|
| `none` | No apparent protection | Direct vulnerabilities, no
```

</details>
