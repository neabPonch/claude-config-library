---
name: davila7__claude-code-templates__skill
source: https://github.com/davila7/claude-code-templates/blob/0eaf1d75ad96b511bcdd975988c002dbafcbcc2e/cli-tool/components/skills/productivity/skill-developer/SKILL.md
repo: davila7/claude-code-templates
kind: skill
stars: 28095
last_pushed: 2026-06-16T04:34:57Z
license: mit
score: 9
domains: [agents-ai, cli-tools, developer-experience]
tags: [meta-skill, guardrails, automation]
curated: 2026-06-16
curated_by: config-scout
---

# davila7/claude-code-templates — skill

**Why it's worth keeping:** It outlines a sophisticated two-hook architecture (proactive vs. reactive) and includes advanced patterns like session-aware state tracking to prevent 'nagging' behaviors.

**Summary:** A meta-skill guide that defines the architectural framework for designing, testing, and implementing Claude Code skills using hooks.

**Source credibility:** High; part of a highly starred repository indicating it is a foundational template for the Claude Code community.

**Recency:** Current; references 2025 workflow updates and modern progressive disclosure techniques.

**Source:** [davila7/claude-code-templates/cli-tool/components/skills/productivity/skill-developer/SKILL.md](https://github.com/davila7/claude-code-templates/blob/0eaf1d75ad96b511bcdd975988c002dbafcbcc2e/cli-tool/components/skills/productivity/skill-developer/SKILL.md) · 28095★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skill-developer
description: Create and manage Claude Code skills following Anthropic best practices. Use when creating new skills, modifying skill-rules.json, understanding trigger patterns, working with hooks, debugging skill activation, or implementing progressive disclosure. Covers skill structure, YAML frontmatter, trigger types (keywords, intent patterns, file paths, content patterns), enforcement levels (block, suggest, warn), hook mechanisms (UserPromptSubmit, PreToolUse), session tracking, and the 500-line rule.
---

# Skill Developer Guide

## Purpose

Comprehensive guide for creating and managing skills in Claude Code with auto-activation system, following Anthropic's official best practices including the 500-line rule and progressive disclosure pattern.

## When to Use This Skill

Automatically activates when you mention:
- Creating or adding skills
- Modifying skill triggers or rules
- Understanding how skill activation works
- Debugging skill activation issues
- Working with skill-rules.json
- Hook system mechanics
- Claude Code best practices
- Progressive disclosure
- YAML frontmatter
- 500-line rule

---

## System Overview

### Two-Hook Architecture

**1
```

</details>
