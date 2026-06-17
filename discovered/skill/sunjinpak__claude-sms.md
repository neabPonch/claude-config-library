---
name: sunjinpak__claude-sms
source: https://github.com/sunjinpak/claude-sms/blob/f7c5e335cea2b3ddcb893595219235f982f4a1cf/skill.md
repo: sunjinpak/claude-sms
kind: skill
stars: 0
last_pushed: 2026-05-20T23:25:30Z
license: mit
score: 8
domains: [cli-tools, macOS, automation]
tags: [sms, macos, bulk-messaging, continuity]
curated: 2026-06-15
curated_by: config-scout
---

# sunjinpak/claude-sms — skill

**Why it's worth keeping:** Provides a high-quality human-in-the-loop workflow with dry runs and explicit approval steps; includes sophisticated SQLite queries to verify message delivery status directly from the OS.

**Summary:** Automates bulk SMS/iMessage sending via macOS continuity, including reply scanning by querying the local Messages database.

**Source credibility:** Low star count but shows deep technical understanding of macOS internals (chat.db/osascript).

**Recency:** Current; addresses modern Apple continuity and messaging behaviors.

**Source:** [sunjinpak/claude-sms/skill.md](https://github.com/sunjinpak/claude-sms/blob/f7c5e335cea2b3ddcb893595219235f982f4a1cf/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sms
description: Send SMS in bulk from this Mac via iPhone+Mac SMS forwarding, and (optionally) scan replies in the local Messages database. Use when the user wants to send a personalized text message to one or more recipients ("send a text to ...", "remind everyone in this list", "text the team about ..."). Free, no external API.
model: sonnet
category: automation
version: 1.0.0
---

# sms Skill

Send SMS from a macOS Mac, routed through the user's iPhone over Continuity. Free (uses the user's existing mobile plan). Drives Messages.app via `osascript`. Reply scanning is via `~/Library/Messages/chat.db`.

## When to use

- User asks to text one or more people.
- User has a list of phone numbers and wants to send each a personalized message.
- User wants to check whether previously-texted people have replied.

## When NOT to use

- Sending to a single number where the user could just type it manually — only use the skill if there are multiple recipients, or the user wants the message logged, or wants a reply scan.
- Marketing / unsolicited outreach — flag the legal issue, don't proceed.
- When the user wants reliable delivery with anonymity — recommend Twilio instead.

##
```

</details>
