---
name: VoltAgent__awesome-claude-code-subagents
source: https://github.com/VoltAgent/awesome-claude-code-subagents/blob/2f9cf8b9562dcc235cc2296bda6df82d60e800be/CLAUDE.md
repo: VoltAgent/awesome-claude-code-subagents
kind: claude-md
stars: 21819
last_pushed: 2026-05-27T10:45:40Z
license: mit
score: 8
domains: [agents-ai, cli-tools, developer-experience]
tags: [orchestration, subagents, meta-framework]
curated: 2026-06-15
curated_by: config-scout
---

# VoltAgent/awesome-claude-code-subagents — claude-md

**Why it's worth keeping:** The schema used to define agents (name, description, tools) is an excellent template for creating scalable AI assistant libraries. The explicit mapping of roles to specific tool permissions is a highly transferable pattern.

**Summary:** Defines a formal framework for specialized subagent orchestration using markdown files with YAML frontmatter. It provides structured role-based tool permissioning and storage definitions.

**Source credibility:** High; repository has significant star count and recent maintenance activity.

**Recency:** Current; explicitly designed for Claude Code's subagent capabilities.

**Source:** [VoltAgent/awesome-claude-code-subagents/CLAUDE.md](https://github.com/VoltAgent/awesome-claude-code-subagents/blob/2f9cf8b9562dcc235cc2296bda6df82d60e800be/CLAUDE.md) · 21819★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a curated collection of Claude Code subagent definitions - specialized AI assistants for specific development tasks. Subagents are markdown files with YAML frontmatter that Claude Code can load and use.

## Repository Structure

```
categories/
  01-core-development/     # Backend, frontend, fullstack, mobile, etc.
  02-language-specialists/ # Language/framework experts (TypeScript, Python, etc.)
  03-infrastructure/       # DevOps, cloud, Kubernetes, etc.
  04-quality-security/     # Testing, security auditing, code review
  05-data-ai/              # ML, data engineering, AI specialists
  06-developer-experience/ # Tooling, documentation, DX optimization
  07-specialized-domains/  # Blockchain, IoT, fintech, gaming
  08-business-product/     # Product management, business analysis
  09-meta-orchestration/   # Multi-agent coordination
  10-research-analysis/    # Research and analysis specialists
```

## Subagent File Format

Each subagent follows this template:

```yaml
---
name: agent-name
description: When this agent should be invoked
```

</details>
