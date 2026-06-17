---
name: catlog22__Claude-Code-Workflow__skill
source: https://github.com/catlog22/Claude-Code-Workflow/blob/5ff5e86257b7e55aec93663930e21ff274f4c023/.codex/skills/spec-add/SKILL.md
repo: catlog22/Claude-Code-Workflow
kind: skill
stars: 2113
last_pushed: 2026-05-14T15:48:37Z
license: mit
score: 9
domains: [cli-tools, developer-experience, ai-agents]
tags: [context-management, rules-engine, workflow-automation, documentation]
curated: 2026-06-15
curated_by: config-scout
---

# catlog22/Claude-Code-Workflow — skill

**Why it's worth keeping:** The hierarchical categorization system (dimension/scope/type) provides a professional way to prevent context rot. The implementation logic includes advanced argument parsing and clear 'Path A/B' decision trees that are easily adaptable for any high-quality agent skill.

**Summary:** A highly structured tool for capturing project context through organized 'specs' (conventions, constraints, and learnings). It uses a dual-mode approach of interactive wizardry and direct CLI execution.

**Source credibility:** High; the source repository is highly starred and specialized in multi-agent orchestration.

**Recency:** Current; utilizes modern tool-calling patterns like request_user_input.

**Source:** [catlog22/Claude-Code-Workflow/.codex/skills/spec-add/SKILL.md](https://github.com/catlog22/Claude-Code-Workflow/blob/5ff5e86257b7e55aec93663930e21ff274f4c023/.codex/skills/spec-add/SKILL.md) · 2113★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spec-add
description: Add specs, conventions, constraints, or learnings to project guidelines interactively or automatically
argument-hint: "[-y|--yes] [--type <convention|constraint|learning>] [--category <category>] [--dimension <specs|personal>] [--scope <global|project>] [--interactive] \"rule text\""
allowed-tools: request_user_input, Read, Write, Edit, Bash, Glob, Grep
---

# Spec Add Command

## Overview

Unified command for adding specs one at a time. Supports both interactive wizard mode and direct CLI mode.

**Key Features**:
- Supports both project specs and personal specs
- Scope selection (global vs project) for personal specs
- Category-based organization for workflow stages
- Interactive wizard mode with smart defaults
- Direct CLI mode with auto-detection of type and category
- Auto-confirm mode (`-y`/`--yes`) for scripted usage

## Use Cases

1. **During Session**: Capture important decisions as they're made
2. **After Session**: Reflect on lessons learned before archiving
3. **Proactive**: Add team conventions or architectural rules
4. **Interactive**: Guided wizard for adding rules with full control over dimension, scope, and category

## Usage

```bash
```

</details>
