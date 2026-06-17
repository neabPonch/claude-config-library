---
name: evanpurkhiser__dots-personal__skill
source: https://github.com/evanpurkhiser/dots-personal/blob/57698a676cdad7386263138f4fd5646ddfc89a15/base/agents/skills/notify-evan/SKILL.md
repo: evanpurkhiser/dots-personal
kind: skill
stars: 33
last_pushed: 2026-06-11T19:43:57Z
license: mit
score: 7
domains: [agents-ai, cli-tools, productivity]
tags: [notification, human-in-the-loop, idle-detection]
curated: 2026-06-16
curated_by: config-scout
---

# evanpurkhiser/dots-personal — skill

**Why it's worth keeping:** The 'one-way' communication constraint prevents agent stalling, while the idle-check logic ensures notifications respect user presence.

**Summary:** Defines a one-way notification protocol that uses macOS idle-time telemetry to choose between terminal output or push notifications.

**Source credibility:** Personal dotfile repository with recent maintenance.

**Recency:** Current; utilizes modern macOS shell commands for system state detection.

**Source:** [evanpurkhiser/dots-personal/base/agents/skills/notify-evan/SKILL.md](https://github.com/evanpurkhiser/dots-personal/blob/57698a676cdad7386263138f4fd5646ddfc89a15/base/agents/skills/notify-evan/SKILL.md) · 33★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: notify-evan
description: Send Evan a Telegram notification via purkhiser-bot. Use proactively when Evan is AFK or has said he'll be away and something important needs his attention — SSH agent auth prompts, blocked tasks, errors requiring a decision, long-running tasks completing, or any situation where work cannot proceed without him.
---

## One-way channel — Evan cannot reply

This is a **one-way** notification channel. purkhiser-bot delivers messages to
Evan's phone, but there is **no back-channel** for him to reply through it.

- Notifications must be **statements**, not questions.
- **Never pause** waiting for an answer to a notification — no reply is ever coming.
- If a decision is needed:
  - Prefer making the call yourself with whatever judgment you have, and proceed.
  - If you genuinely cannot proceed, stop and surface the question in your
    terminal output where Evan will see it next time he checks — but do not
    block waiting for a Telegram reply.

## Checking if Evan is AFK

On macOS, always check keyboard/mouse idle time before notifying. If Evan is
actively at his machine, print a message to the terminal instead and wait — only
send a push notification
```

</details>
