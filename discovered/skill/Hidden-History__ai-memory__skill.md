---
name: Hidden-History__ai-memory__skill
source: https://github.com/Hidden-History/ai-memory/blob/886adaf46db67223ad1623eab6e7f8c32cc2927b/.claude/skills/aim-settings/SKILL.md
repo: Hidden-History/ai-memory
kind: skill
stars: 38
last_pushed: 2026-06-15T04:26:51Z
license: mit
score: 8
domains: [agents-ai, cli-tools, vector-databases]
tags: [memory-management, observability, configuration]
curated: 2026-06-15
curated_by: config-scout
---

# Hidden-History/ai-memory — skill

**Why it's worth keeping:** Demonstrates professional-grade pattern for role-based resource management (token budgeting per agent) and high-precision retrieval tuning (similarity/dedup thresholds).

**Summary:** Provides observability into a semantic memory system's configuration, including vector DB thresholds and service endpoints.

**Source credibility:** Good; the repository is active and demonstrates a mature, sophisticated architecture for AI memory.

**Recency:** Current; addresses modern requirements for persistent context in agentic workflows.

**Source:** [Hidden-History/ai-memory/.claude/skills/aim-settings/SKILL.md](https://github.com/Hidden-History/ai-memory/blob/886adaf46db67223ad1623eab6e7f8c32cc2927b/.claude/skills/aim-settings/SKILL.md) · 38★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aim-settings
description: 'Display current memory system configuration and settings'
allowed-tools: Read
---

# Memory Settings - Configuration Viewer

Display the current configuration of the AI Memory Module, including collections, types, thresholds, token budgets, and service endpoints.

## Activation

```text
# Show all memory settings
/aim-settings

# Show specific section
/aim-settings --section collections
/aim-settings --section types
/aim-settings --section thresholds
/aim-settings --section services
/aim-settings --section agents
```

## Configuration Sections

### Collections
Shows the 3 Memory System V2.0 collections:
- **code-patterns** - Project-specific implementation patterns
- **conventions** - Cross-project shared conventions
- **discussions** - Decision context and session summaries

### Memory Types (14 total)
Organized by collection:
- code-patterns: `implementation`, `error_fix`, `refactor`, `file_pattern`
- conventions: `rule`, `guideline`, `port`, `naming`, `structure`
- discussions: `decision`, `session`, `blocker`, `preference`, `context`

### Thresholds
- **similarity_threshold** - Minimum relevance score for search results (default: 0.7)
- **de
```

</details>
