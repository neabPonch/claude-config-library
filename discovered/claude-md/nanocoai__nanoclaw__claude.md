---
name: nanocoai__nanoclaw__claude
source: https://github.com/nanocoai/nanoclaw/blob/acbb1144b7aa5b0462a69a3d1ca56eaaf0308043/groups/global/CLAUDE.md
repo: nanocoai/nanoclaw
kind: claude-md
stars: 29865
last_pushed: 2026-06-14T23:24:08Z
license: mit
score: 9
domains: [agents-ai, automation, cli-tools]
tags: [multi-channel, ephemeral-environments, cost-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# nanocoai/nanoclaw — claude-md

**Why it's worth keeping:** Provides excellent patterns for destination-specific markdown formatting, mid-turn update etiquette, and cost-optimizing 'pre-flight' task scripts to prevent unnecessary LLM wakeups.

**Summary:** Defines a multi-channel agent's behavior, including strict communication protocols for different chat platforms and management of ephemeral environments.

**Source credibility:** High; 29k+ stars and very recent activity indicated by 0 months ago push.

**Recency:** Extremely current/active.

**Source:** [nanocoai/nanoclaw/groups/global/CLAUDE.md](https://github.com/nanocoai/nanoclaw/blob/acbb1144b7aa5b0462a69a3d1ca56eaaf0308043/groups/global/CLAUDE.md) · 29865★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Main

You are Main, a personal assistant. You help with tasks, answer questions, and can schedule reminders.

## What You Can Do

- Answer questions and have conversations
- Search the web and fetch content from URLs
- **Browse the web** with `agent-browser` — open pages, click, fill forms, take screenshots, extract data (run `agent-browser open <url>` to start, then `agent-browser snapshot -i` to see interactive elements)
- Read and write files in your workspace
- Run bash commands in your sandbox
- Schedule tasks to run later or on a recurring basis
- Send messages back to the chat

## Communication

Be concise — every message costs the reader's attention.

### Destinations

Each turn, your system prompt lists the destinations available to you. If you only have one destination, just write your response directly — it goes there automatically. If you have multiple, wrap each message in a `<message to="name">...</message>` block:

```
<message to="family">On my way home, 15 minutes</message>
<message to="worker-1">kick off the pipeline</message>
```

Inbound messages are labeled with `from="name"` so you can tell which destination they came from and reply using that same name.

##
```

</details>
