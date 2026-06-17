---
name: ColtonWilley__ue-llm-toolkit__claude-default
source: https://github.com/ColtonWilley/ue-llm-toolkit/blob/9f6a0f7930db4751d915b8f6f1a87e809895791e/Plugin/UELLMToolkit/CLAUDE.md.default
repo: ColtonWilley/ue-llm-toolkit
kind: claude-md
stars: 93
last_pushed: 2026-04-02T22:27:55Z
license: mit
score: 9
domains: [game-engine, c++, ai-agents, tooling]
tags: [unreal-engine, context-management, automation]
curated: 2026-06-16
curated_by: config-scout
---

# ColtonWilley/ue-llm-toolkit — claude-md

**Why it's worth keeping:** The `prep <domain>` pattern is a high-level technique for managing large project contexts, and the inclusion of explicit security/validation rules is critical for agentic automation tools.

**Summary:** This file establishes a sophisticated domain-driven knowledge system using 'prep' commands to manage LLM context efficiently. It also enforces strict C++ implementation standards and provides clear patterns for extending the plugin.

**Source credibility:** Highly specialized niche toolset with recent activity and meaningful star count in the Unreal Engine ecosystem.

**Recency:** Very current; targets UE 5.7 and utilizes modern MCP-style architecture.

**Source:** [ColtonWilley/ue-llm-toolkit/Plugin/UELLMToolkit/CLAUDE.md.default](https://github.com/ColtonWilley/ue-llm-toolkit/blob/9f6a0f7930db4751d915b8f6f1a87e809895791e/Plugin/UELLMToolkit/CLAUDE.md.default) · 93★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# UE LLM Toolkit - Claude Code Instructions for Unreal Engine 5.7

This file provides guidance to Claude Code when working with the UE LLM Toolkit plugin and Unreal Engine 5.7 projects.

## Setup

Copy this file to `CLAUDE.md` in the same directory and customize the build paths for your system.

## Project Overview

**UE LLM Toolkit** is an Unreal Engine 5.7 plugin that provides an HTTP REST API for LLM-driven editor automation — 38 tools, 201 operations for Blueprint editing, animation, materials, level management, and more.

### Key Directories
- `Source/UELLMToolkit/Private/MCP/` - HTTP server and tool implementations
- `Source/UELLMToolkit/Private/MCP/Tools/` - Individual tool classes
- `Source/UELLMToolkit/Private/Tests/` - Automation tests
- `Resources/mcp-bridge/` - Node.js MCP bridge

### Build Commands
```bash
# Build plugin - customize these paths for your system:
# - UE_PATH: Your Unreal Engine installation
# - PLUGIN_PATH: Path to UELLMToolkit.uplugin
# - OUTPUT_PATH: Temporary build output directory

"<UE_PATH>/Engine/Build/BatchFiles/RunUAT.bat" BuildPlugin -Plugin="<PLUGIN_PATH>/UELLMToolkit.uplugin" -Package="<OUTPUT_PATH>" -TargetPlatforms=Win64 -Rocket

# Run test
```

</details>
