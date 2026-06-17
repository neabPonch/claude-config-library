---
name: jackwener__tg-cli
source: https://github.com/jackwener/tg-cli/blob/b54a14da62a5e03cbd6d65d4b8dc95932194d2d0/SKILL.md
repo: jackwener/tg-cli
kind: skill
stars: 254
last_pushed: 2026-03-15T08:46:30Z
license: apache-2.0
score: 9
domains: [cli-tools, messaging, automation]
tags: [telegram, sync, chat]
curated: 2026-06-15
curated_by: config-scout
---

# jackwener/tg-cli — skill

**Why it's worth keeping:** Features 'Common Patterns' recipes specifically for agents and explicitly prioritizes structured YAML output to ensure reliable parsing and state management.

**Summary:** Provides comprehensive instructions for interacting with a Telegram CLI, including synchronization strategies and authentication.

**Source credibility:** Strong; active repository with significant community interest (254 stars).

**Recency:** Current/Modern.

**Source:** [jackwener/tg-cli/SKILL.md](https://github.com/jackwener/tg-cli/blob/b54a14da62a5e03cbd6d65d4b8dc95932194d2d0/SKILL.md) · 254★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tg-cli
description: CLI skill for Telegram to sync chats, search messages, filter keywords, and monitor groups from the terminal
author: jackwener
version: "0.5.4"
tags:
  - telegram
  - tg
  - chat
  - monitor
  - cli
---

# tg-cli Skill

CLI tool for Telegram — sync chats, search messages, filter keywords, send messages, and monitor groups.

## Prerequisites

```bash
# Install (requires Python 3.10+)
uv tool install kabi-tg-cli
# Or: pipx install kabi-tg-cli

# Upgrade to latest (recommended to avoid API errors)
uv tool upgrade kabi-tg-cli
# Or: pipx upgrade kabi-tg-cli
```

## Authentication

Uses your Telegram account (MTProto). Built-in Telegram Desktop API credentials are used by default — no application needed.

```bash
tg chats              # First run: enter phone + verification code
tg whoami             # Check current user

# Optional: use your own app credentials
export TG_API_ID=123456
export TG_API_HASH=your_telegram_app_hash
```

## Command Reference

### Telegram Operations

```bash
tg chats                          # List joined chats
tg chats --type group             # Filter by type
tg status                         # Check auth/session status
tg statu
```

</details>
