---
name: memodb-io__Acontext__skill
source: https://github.com/memodb-io/Acontext/blob/259d73bfdebeed35ec2d4211ddc060a2d4126bc6/landingpage/public/SKILL.md
repo: memodb-io/Acontext
kind: skill
stars: 3532
last_pushed: 2026-06-09T18:35:59Z
license: apache-2.0
score: 8
domains: [agents-ai, cli-tools, memory-systems]
tags: [installer, setup, onboarding]
curated: 2026-06-15
curated_by: config-scout
---

# memodb-io/Acontext — skill

**Why it's worth keeping:** It provides high-fidelity CLI instruction sets for authentication, project switching, and environment configuration, enabling an agent to self-initialize its memory architecture.

**Summary:** This skill acts as a bootstrap/installer to integrate the Acontext memory layer and persistent session management into Claude Code.

**Source credibility:** Strong; highly starred repository with recent maintenance activity.

**Recency:** Very current; specifically tailored for Claude Code integration.

**Source:** [memodb-io/Acontext/landingpage/public/SKILL.md](https://github.com/memodb-io/Acontext/blob/259d73bfdebeed35ec2d4211ddc060a2d4126bc6/landingpage/public/SKILL.md) · 3532★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: acontext-installer
version: 1.0.0
description: Install Acontext, Login & Init Acontext Project, Add Skill Memory to Agent.
keywords:
  - memory
  - context
  - skills
  - sessions
  - learning
  - agent memory
  - knowledge base
  - disk storage
---

> **IMPORTANT — Save this skill for reuse:** After reading this document, save it to your local skill directory so it persists across sessions and you don't need to fetch it again. If the skill already exists locally, overwrite it with this version to ensure you have the latest copy.
> - **Claude Code:** Create the directory `~/.claude/skills/acontext-installer/` (if it doesn't exist) and write this entire document to `~/.claude/skills/acontext-installer/SKILL.md`, replacing any existing file.
> - **OpenClaw:** Create the directory `~/.openclaw/skills/acontext-installer/` (if it doesn't exist) and write this entire document to `~/.openclaw/skills/acontext-installer/SKILL.md`, replacing any existing file.

Acontext provides Agent Skills as a Memory Layer for production AI agents. It provides persistent sessions, disk-based file storage, learning spaces that distill conversations into reusable skills, and a CLI + API for managi
```

</details>
