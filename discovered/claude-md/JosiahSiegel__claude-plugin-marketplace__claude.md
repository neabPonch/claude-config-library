---
name: JosiahSiegel__claude-plugin-marketplace__claude
source: https://github.com/JosiahSiegel/claude-plugin-marketplace/blob/a775642a55a1ff79fe350d67f697d5f49e2171eb/scripts/CLAUDE.md
repo: JosiahSiegel/claude-plugin-marketplace
kind: claude-md
stars: 45
last_pushed: 2026-05-28T04:04:26Z
license: mit
score: 8
domains: [cli-tools, automation]
tags: [workflow, versioning, metadata-sync]
curated: 2026-06-16
curated_by: config-scout
---

# JosiahSiegel/claude-plugin-marketplace — claude-md

**Why it's worth keeping:** Includes highly structured 'AI Agent Workflows' and exhaustive CLI parameter documentation that prevents hallucination of arguments. Establishes clear 'Source of Truth' rules, which is essential for agents managing multi-file dependencies.

**Summary:** Provides precise command-line usage and state-management logic for synchronizing plugin metadata across multiple files. It defines specific validation gates and operational workflows to ensure data integrity during agent-led updates.

**Source credibility:** Moderate; a specialized marketplace project with decent community traction (45 stars).

**Recency:** Current; utilizes modern CLI and script-driven workflows suitable for Claude Code.

**Source:** [JosiahSiegel/claude-plugin-marketplace/scripts/CLAUDE.md](https://github.com/JosiahSiegel/claude-plugin-marketplace/blob/a775642a55a1ff79fe350d67f697d5f49e2171eb/scripts/CLAUDE.md) · 45★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Version Tracking for AI Agents

This document describes how AI agents should use the `version_ops.py` script to manage plugin versions in the Claude Plugin Marketplace.

## Overview

The marketplace uses two locations for plugin versions:
1. **`.claude-plugin/marketplace.json`** - Central registry with all plugin metadata
2. **`plugins/<plugin-name>/.claude-plugin/plugin.json`** - Individual plugin configuration

Both locations MUST have matching versions. The central marketplace also mirrors plugin keywords from each plugin's `plugin.json`; the plugin-owned `keywords` array is the source of truth for keyword sync. The `version_ops.py` script ensures consistency.

## File Locations

```
claude-code-marketplace/
├── .claude-plugin/
│   └── marketplace.json          # Central version registry
├── plugins/
│   ├── bash-master/
│   │   └── .claude-plugin/
│   │       └── plugin.json       # Plugin-owned version and keywords
│   ├── ffmpeg-master/
│   │   └── .claude-plugin/
│   │       └── plugin.json
│   └── ...                       # registered plugins
└── scripts/
    ├── version_ops.py            # Main Python script
    ├── version-tracker.sh        # Bash wrapper
    └── CLAUD
```

</details>
