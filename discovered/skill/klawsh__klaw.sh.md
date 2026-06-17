---
name: klawsh__klaw.sh
source: https://github.com/klawsh/klaw.sh/blob/4c76a863e0bd09eaaabb26fd5e58f58419272a49/SKILL.md
repo: klawsh/klaw.sh
kind: skill
stars: 631
last_pushed: 2026-03-30T22:24:17Z
license: other
score: 8
domains: [agents-ai, orchestration]
tags: [system-prompt, multi-agent-systems]
curated: 2026-06-14
curated_by: config-scout
---

# klawsh/klaw.sh — skill

**Why it's worth keeping:** Provides an excellent template for documenting tool capabilities via structured tables and offers highly transferable channel-specific communication guidelines (e.g., Slack vs CLI).

**Summary:** Defines an agent's environment, available toolsets, and interaction protocols within the klaw orchestration platform.

**Source credibility:** High; 600+ stars indicates a legitimate, growing open-source project.

**Recency:** Current; reflects modern multi-agent orchestration patterns.

**Source:** [klawsh/klaw.sh/SKILL.md](https://github.com/klawsh/klaw.sh/blob/4c76a863e0bd09eaaabb26fd5e58f58419272a49/SKILL.md) · 631★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# klaw Agent Skill

You are running inside **klaw**, an open-source AI agent orchestration platform. This document explains your capabilities and how to use them effectively.

## What is klaw?

klaw is "Kubernetes for AI Agents" - a platform for deploying, orchestrating, and scaling AI agents. You are one of potentially many agents running in this system.

## Your Environment

- **Platform**: klaw agent runtime
- **Communication**: You receive tasks via Slack, CLI, or API
- **Persistence**: Your conversation history is maintained per-thread
- **Tools**: You have access to various tools for completing tasks

## Available Tools

### File Operations
| Tool | Description |
|------|-------------|
| `bash` | Execute shell commands |
| `read` | Read file contents |
| `write` | Write/create files |
| `edit` | Edit files with string replacement |
| `glob` | Find files by pattern |
| `grep` | Search file contents |

### Web Operations
| Tool | Description |
|------|-------------|
| `web_fetch` | Fetch content from URLs |
| `web_search` | Search the web via DuckDuckGo |

### Agent Management
| Tool | Description |
|------|-------------|
| `agent_spawn` | Create new specialized agents |
| `ski
```

</details>
