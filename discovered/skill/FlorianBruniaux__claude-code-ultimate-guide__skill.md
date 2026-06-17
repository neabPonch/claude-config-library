---
name: FlorianBruniaux__claude-code-ultimate-guide__skill
source: https://github.com/FlorianBruniaux/claude-code-ultimate-guide/blob/24baa819a8ee505d6261a24167ec7d5c77abb493/examples/skills/design-patterns/SKILL.md
repo: FlorianBruniaux/claude-code-ultimate-guide
kind: skill
stars: 5016
last_pushed: 2026-06-11T13:38:01Z
license: cc-by-sa-4.0
score: 9
domains: [web-frontend, software-architecture, typescript]
tags: [design-patterns, refactoring, stack-aware]
curated: 2026-06-15
curated_by: config-scout
---

# FlorianBruniaux/claude-code-ultimate-guide — skill

**Why it's worth keeping:** The 'Stack Adaptation' logic is exceptional, instructing the agent to prioritize framework-native idioms (e.g., React Context over Singletons) rather than generic theory. The multi-mode workflow (Detection, Suggestion, Evaluation) provides a highly structured operational framework for an agent.

**Summary:** A sophisticated skill that enables Claude Code to detect, suggest, and evaluate GoF design patterns with framework-specific context.

**Source credibility:** High; part of a popular, well-maintained repository with significant community validation (5k+ stars).

**Recency:** Very current, targeting modern TypeScript and JS ecosystem frameworks.

**Source:** [FlorianBruniaux/claude-code-ultimate-guide/examples/skills/design-patterns/SKILL.md](https://github.com/FlorianBruniaux/claude-code-ultimate-guide/blob/24baa819a8ee505d6261a24167ec7d5c77abb493/examples/skills/design-patterns/SKILL.md) · 5016★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: design-patterns
description: "Detect, suggest, and evaluate GoF design patterns in TypeScript/JavaScript codebases. Use when refactoring code, applying singleton/factory/observer/strategy patterns, reviewing pattern quality, or finding stack-native alternatives for React, Angular, NestJS, and Vue."
allowed-tools: Read Grep Glob mcp__grepai__grepai_search
context: fork
agent: specialist
effort: high
---

# Design Patterns Analyzer Skill

**Purpose**: Detect, suggest, and evaluate Gang of Four (GoF) design patterns in TypeScript/JavaScript codebases with stack-aware adaptations.

## Core Capabilities

1. **Stack Detection**: Identify primary framework/library (React, Angular, NestJS, Vue, Express, RxJS, Redux, ORMs)
2. **Pattern Detection**: Find existing implementations of 23 GoF patterns
3. **Smart Suggestions**: Recommend patterns to fix code smells, using stack-native idioms when available
4. **Quality Evaluation**: Assess pattern implementation quality against best practices

## Operating Modes

### Mode 1: Detection

**Trigger**: User requests pattern detection or analysis
**Output**: JSON report of patterns found with confidence scores and stack context

**Workflow**
```

</details>
