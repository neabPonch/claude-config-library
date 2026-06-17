---
name: javimosch__supercli__skill
source: https://github.com/javimosch/supercli/blob/3e84a407c20a288daffb47a043b41bb53d91c909/plugins/mcfly/skills/quickstart/SKILL.md
repo: javimosch/supercli
kind: skill
stars: 39
last_pushed: 2026-06-15T05:47:57Z
license: mit
score: 7
domains: [cli-tools, productivity]
tags: [shell-history, terminal]
curated: 2026-06-15
curated_by: config-scout
---

# javimosch/supercli — skill

**Why it's worth keeping:** Uses a structured pattern of mapping natural language 'Usage Examples' directly to specific CLI commands, which is ideal for agentic tool-use.

**Summary:** Integrates the mcfly smart shell history tool, enabling Claude to search and analyze command history via neural ranking.

**Source credibility:** Part of a specialized collection with active development and high utility density.

**Recency:** Current; utilizes modern Rust-based terminal automation patterns.

**Source:** [javimosch/supercli/plugins/mcfly/skills/quickstart/SKILL.md](https://github.com/javimosch/supercli/blob/3e84a407c20a288daffb47a043b41bb53d91c909/plugins/mcfly/skills/quickstart/SKILL.md) · 39★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mcfly
description: Use this skill when the user wants to search shell history, find a command they ran before, or explore their terminal history with smart ranking.
---

# mcfly Plugin

Smart shell history search. Replaces Ctrl+R with neural ranking that learns from context, frequency, and recency.

## Commands

### Search
- `mcfly history search <query>` — Search shell history with neural ranking

### Manage
- `mcfly history dump` — Dump all shell history entries
- `mcfly history train` — Train mcfly model on current history

## Usage Examples
- "Find that docker command I ran yesterday"
- "Search my history for git rebase commands"
- "Dump my entire shell history"
- "Train mcfly on my history"

## Installation

```bash
cargo install mcfly
```

For shell integration, add to your `.bashrc`:

```bash
eval "$(mcfly init bash)"
```

## Examples

```bash
# Search history for a command
mcfly search docker compose

# Dump all history (json lines)
mcfly dump

# Train on history
mcfly train --train-all

# Shell integration (in .bashrc)
eval "$(mcfly init bash)"
```

## Key Features
- Neural network ranking for relevant results
- Works with bash, zsh, and fish
- Time-based and fre
```

</details>
