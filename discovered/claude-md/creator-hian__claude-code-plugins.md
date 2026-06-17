---
name: creator-hian__claude-code-plugins
source: https://github.com/creator-hian/claude-code-plugins/blob/d233841844bee7d81a94c3762477d341ba068092/CLAUDE.md
repo: creator-hian/claude-code-plugins
kind: claude-md
stars: 9
last_pushed: 2026-04-23T09:31:44Z
license: unknown
score: 9
domains: [ai-agents, cli-tools, architecture]
tags: [progressive-disclosure, plugin-system, context-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# creator-hian/claude-code-plugins — claude-md

**Why it's worth keeping:** The '3-Level Progressive Disclosure' system for managing context windows via L1/L2/L3 layers is an elite, transferable pattern. It also provides a clear distinction between procedural skills and complex agent workflows.

**Summary:** Defines a hierarchical plugin architecture designed to extend Claude Code with specialized skills and agents.

**Source credibility:** Niche repository with highly sophisticated architectural patterns despite low star count.

**Recency:** Highly current; represents the cutting edge of agentic tool-use architectures.

**Source:** [creator-hian/claude-code-plugins/CLAUDE.md](https://github.com/creator-hian/claude-code-plugins/blob/d233841844bee7d81a94c3762477d341ba068092/CLAUDE.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Claude Code Plugin Marketplace** - a collection of custom plugins that extend Claude Code's capabilities through Skills, Agents, Commands, and Hooks. The repository currently contains 7 plugins with 24 skills total.

## Repository Structure

```
claude-code-plugins/
├── csharp-plugin/          # C# async patterns, code style, XML docs
├── unity-plugin/           # Unity game development (13 skills)
├── codex-plugin/           # OpenAI Codex CLI integration
├── gemini-plugin/          # Google Gemini CLI integration
├── ai-orchestration-plugin/# Multi-AI orchestration (Claude+Codex+Gemini)
├── agent-team-plugin/      # Agent team planning & adversarial review
├── tools/
│   ├── create_plugin.py    # Plugin creation script
│   └── plugin-template/    # Template for new plugins
└── docs/                   # Architecture documentation
```

## Plugin Architecture

Each plugin follows this structure:
```
plugin-name/
├── .claude-plugin/
│   └── plugin.json         # Metadata (name, version, author)
├── agents/                 # Specialized
```

</details>
