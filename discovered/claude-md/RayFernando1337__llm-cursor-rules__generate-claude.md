---
name: RayFernando1337__llm-cursor-rules__generate-claude
source: https://github.com/RayFernando1337/llm-cursor-rules/blob/d31bec10c7c4f9cce5f7d703184bb3fd1eb9d8c5/generate-claude.md
repo: RayFernando1337/llm-cursor-rules
kind: claude-md
stars: 888
last_pushed: 2025-11-26T16:49:15Z
license: mit
score: 9
domains: [ai-agents, devops, developer-productivity]
tags: [meta-instruction, hierarchical-rules, claude-code]
curated: 2026-06-15
curated_by: config-scout
---

# RayFernando1337/llm-cursor-rules — claude-md

**Why it's worth keeping:** It utilizes a hierarchical approach (Root vs Subdirectory) for large codebases and includes highly practical 'Quick Find' patterns using ripgrep for rapid navigation.

**Summary:** A sophisticated meta-instructional framework that directs Claude Code to analyze a repository and construct a multi-layered hierarchy of CLAUDE.md files.

**Source credibility:** Highly regarded repository with significant community interest (888 stars).

**Recency:** Current; it explicitly incorporates advanced Claude Code features like MCP, Hooks, and Subagents.

**Source:** [RayFernando1337/llm-cursor-rules/generate-claude.md](https://github.com/RayFernando1337/llm-cursor-rules/blob/d31bec10c7c4f9cce5f7d703184bb3fd1eb9d8c5/generate-claude.md) · 888★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Task: Analyze this codebase and generate a hierarchical CLAUDE.md system optimized for Claude Code

## Critical Context: Claude Code is Different from Other Agents

Claude Code has unique capabilities that set it apart from generic AGENTS.md:

1. **Strict Instruction Hierarchy**: CLAUDE.md content is treated as **immutable system rules** with strict priority over user prompts
2. **Hierarchical Memory System**: Reads CLAUDE.md files recursively UP from CWD to root, AND discovers them in subdirectories
3. **Hooks System**: Lifecycle hooks (PreToolUse, PostToolUse, UserPromptSubmit, Notification, Stop) for deterministic automation
4. **Model Context Protocol (MCP)**: Native integration with external tools, databases, and APIs
5. **Custom Slash Commands**: Repeatable workflows stored in `.claude/commands/`
6. **Subagents**: Specialized agents with isolated context windows and tool permissions
7. **Extended Thinking**: Can use long-form reasoning with extended context windows (1M+ tokens)

## Core Principles

1. **CLAUDE.md is AUTHORITATIVE** - Treated as system rules, not suggestions
2. **Modular Sections** - Use clear markdown headers to prevent instruction bleeding
3. **Front-load
```

</details>
