---
name: jeremylongshore__claude-code-plugins-plus-skills__claude
source: https://github.com/jeremylongshore/claude-code-plugins-plus-skills/blob/57b5254bd3d6c39f2d15f3d9750db89b3801d8ab/plugins/community/jeremy-firebase/CLAUDE.md
repo: jeremylongshore/claude-code-plugins-plus-skills
kind: claude-md
stars: 2376
last_pushed: 2026-06-15T02:02:44Z
license: mit
score: 9
domains: [ai-agents, cloud-infrastructure, devops-automation, firebase]
tags: [agentic-workflows, skill-definition, plugin-architecture, structured-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# jeremylongshore/claude-code-plugins-plus-skills — claude-md

**Why it's worth keeping:** Uses strict structural definitions (YAML frontmatter) to categorize tasks into 'Commands', 'Agents', or 'Skills' while explicitly mapping specific tool permissions (Read/Write/Bash) to operation types.

**Summary:** Defines the architectural standards for building specialized AI-driven command sets, multi-step agents, and auto-triggering skills for Firebase operations.

**Source credibility:** Highly credible; part of a large, actively maintained open-source marketplace with thousands of stars.

**Recency:** Extremely current; uses modern Claude Code terminology and patterns for agentic skills.

**Source:** [jeremylongshore/claude-code-plugins-plus-skills/plugins/community/jeremy-firebase/CLAUDE.md](https://github.com/jeremylongshore/claude-code-plugins-plus-skills/blob/57b5254bd3d6c39f2d15f3d9750db89b3801d8ab/plugins/community/jeremy-firebase/CLAUDE.md) · 2376★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Plugin Overview

**jeremy-firebase** is a production-ready Firebase platform operations plugin with Vertex AI Gemini integration. It provides comprehensive automation for Firebase services including Authentication, Cloud Storage, Hosting, Cloud Functions, Analytics, and AI-powered features.

This plugin is part of the claude-code-plugins marketplace and follows the repository's plugin development standards.

## Plugin Structure

```
jeremy-firebase/
├── .claude-plugin/
│   └── plugin.json              # Plugin metadata and configuration
├── commands/                     # Slash commands for common Firebase operations
├── agents/                       # AI agents for complex Firebase workflows
├── skills/                       # Agent Skills for automatic Firebase task handling
│   └── firebase-vertex-ai/      # Main skill for Firebase + Vertex AI integration
└── examples/                     # Code examples and usage patterns
```

## Quick Commands

### Development Workflow

```bash
# Navigate to plugin directory
cd plugins/community/jeremy-firebase/

# Validate p
```

</details>
