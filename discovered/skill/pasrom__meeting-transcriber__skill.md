---
name: pasrom__meeting-transcriber__skill
source: https://github.com/pasrom/meeting-transcriber/blob/75edcb180def029be42d57555fc64f0de0f1b509/tools/mt-cli/skill.md
repo: pasrom/meeting-transcriber
kind: skill
stars: 55
last_pushed: 2026-06-16T15:50:36Z
license: mit
score: 9
domains: [macOS, cli-tools, dev-experience, security]
tags: [rpc, observability, debug-server]
curated: 2026-06-16
curated_by: config-scout
---

# pasrom/meeting-transcriber — skill

**Why it's worth keeping:** Demonstrates the 'Observer Sidecar' pattern: creating a dedicated debug interface so the agent can inspect system state without requiring human manual verification or screenshots.

**Summary:** Provides an agent with programmatic access to a running application's internal state, health, and visual context via a local RPC/CLI tool.

**Source credibility:** High; well-maintained repository with specialized, professional-grade tooling documentation.

**Recency:** Current; aligns perfectly with modern agentic developer workflows.

**Source:** [pasrom/meeting-transcriber/tools/mt-cli/skill.md](https://github.com/pasrom/meeting-transcriber/blob/75edcb180def029be42d57555fc64f0de0f1b509/tools/mt-cli/skill.md) · 55★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: meeting-transcriber
description: Use when working on the Meeting Transcriber repo and you need to inspect or drive the running dev app from the shell instead of asking the user for screenshots.
---

# Meeting Transcriber — shell-driven inspection

The dev build of Meeting Transcriber can run an embedded debug RPC server.
When it's running, prefer `mt-cli` over asking the user "kannst du screenshot
machen" / "ist das im Menü sichtbar".

## When to use

- You want to know what's in the speaker DB right now → `mt-cli state`
- You want to verify the app is alive after a code change → `mt-cli healthz`
- You want to see what the user sees → `mt-cli screenshot /tmp/x.png`, then Read it
- You're debugging a UI bug and would otherwise have to ask the user to describe state
- You're verifying a fix end-to-end after editing code

Don't use it for production debugging — RPC is `#if !APPSTORE` only.

## How to enable

Either persistent (preferred for repeated dev sessions):

- Settings → Advanced → toggle **Debug RPC Server** on. The server starts
  immediately and survives app relaunches.

Or per-session (one-shot, e.g. for `scripts/test_rpc.sh`):

```bash
MEETINGTRANSCRIBER_DEBUG_RP
```

</details>
