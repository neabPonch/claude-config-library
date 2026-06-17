---
name: fcakyon__claude-codex-settings
source: https://github.com/fcakyon/claude-codex-settings/blob/831a96a749d0e641723105c5d15aa9c8d3c91698/CLAUDE.md
repo: fcakyon/claude-codex-settings
kind: claude-md
stars: 732
last_pushed: 2026-05-28T22:45:28Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [plugin-system, agent-orchestration, specifications]
curated: 2026-06-15
curated_by: config-scout
---

# fcakyon/claude-codex-settings — claude-md

**Why it's worth keeping:** It provides rigorous, schema-driven definitions (YAML/JSON) that allow natural language capabilities to be ported between different agentic environments like Claude Code and Cursor.

**Summary:** A sophisticated specification for a cross-platform plugin ecosystem that standardizes agents, skills, and hooks across multiple AI CLI tools.

**Source credibility:** High; a popular repository (732 stars) used as a personal battle-tested toolset.

**Recency:** Very current, updated within the last month.

**Source:** [fcakyon/claude-codex-settings/CLAUDE.md](https://github.com/fcakyon/claude-codex-settings/blob/831a96a749d0e641723105c5d15aa9c8d3c91698/CLAUDE.md) · 732★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# claude-settings

> `AGENTS.md` and `GEMINI.md` are symlinks to this file for Codex CLI and Gemini CLI compatibility.

Multi-tool plugin marketplace. Each plugin under `plugins/` is independently installable on Claude Code, Codex CLI, Gemini CLI, and Cursor.

## Repo Structure

```
claude-settings/
  CLAUDE.md                              # this file (repo dev guide)
  AGENTS.md -> CLAUDE.md                 # Codex CLI reads this
  GEMINI.md -> CLAUDE.md                 # Gemini CLI reads this
  .claude/CLAUDE.md                      # user-facing global config (synced to ~/.claude/CLAUDE.md)
  .claude/settings.json                  # Claude Code settings
  .claude-plugin/marketplace.json        # Claude Code marketplace
  .agents/plugins/marketplace.json       # Codex CLI marketplace
  .cursor-plugin/marketplace.json        # Cursor marketplace
  .codex/config.toml                     # Codex CLI config
  .github/scripts/                       # repo maintenance scripts
    _helpers.sh                          # shared sync/zip functions
    sync-<vendor>-skills.sh              # per-vendor skill sync
    sync-versions.sh                     # version alignment
    release.sh
```

</details>
