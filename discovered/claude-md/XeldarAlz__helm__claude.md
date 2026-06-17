---
name: XeldarAlz__helm__claude
source: https://github.com/XeldarAlz/helm/blob/c0a041051ec241aab3a86fbbee73f4c1267a4c7c/.claude/CLAUDE.md
repo: XeldarAlz/helm
kind: claude-md
stars: 19
last_pushed: 2026-04-27T17:15:19Z
license: mit
score: 9
domains: [game-dev, unity-engine, ai-agents, automation]
tags: [multi-agent, architectural-constraints, performance-optimization, unity]
curated: 2026-06-14
curated_by: config-scout
---

# XeldarAlz/helm — claude-md

**Why it's worth keeping:** The use of 'Skills' for contextual expertise and the 'Pre/PostToolUse' validation hooks are elite patterns for maintaining high-quality codebases. The strict enforcement of pure C# logic separation from Unity MonoBehaviours provides a highly transferable architectural standard.

**Summary:** This config defines a sophisticated multi-agent orchestration system for Unity that enforces strict architectural and performance constraints. It goes beyond simple coding rules by establishing a framework for agent skills, model routing, and automated validation hooks.

**Source credibility:** A specialized, niche project with recent activity indicating it is a functional automation pipeline.

**Recency:** Very current; specifically optimized for Unity 6 and advanced agentic workflows.

**Source:** [XeldarAlz/helm/.claude/CLAUDE.md](https://github.com/XeldarAlz/helm/blob/c0a041051ec241aab3a86fbbee73f4c1267a4c7c/.claude/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Unity Game Factory — AI Agent Automation System

This project is an AI-powered game development pipeline for Unity 6. It uses multiple coordinated Claude Code agents to take a game idea from concept to implementation.

## Pipeline Overview

1. `/game-idea` → Interactive GDD creation (Game Design Document)
2. `/architect` → Technical Design Document (TDD) with full architecture
3. `/plan-workflow` → Phased execution plan optimized for parallel agent work
4. `/init-project` → Generates lean, game-specific CLAUDE.md at Unity project root
5. `/orchestrate` → Multi-agent orchestrator that executes the plan
6. `/build-game` → Runs the full pipeline end-to-end

## Strict Technical Constraints (All Agents Must Follow)

Detailed rules are in `.claude/rules/` — agents load these automatically. Summary:

- **Pure C# logic**: Game logic in pure C# classes, NOT MonoBehaviours. MonoBehaviours are thin wrappers. (See `rules/architecture.md`)
- **Mandatory tests**: Every logic system must have NUnit/Unity Test Framework tests.
- **No tight coupling**: Systems communicate through interfaces, events, or a message bus. (See `rules/architecture.md`)
- **Zero allocation on hot paths**: No `new`, no b
```

</details>
