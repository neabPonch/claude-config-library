---
name: rbrown101010__rilable
source: https://github.com/rbrown101010/rilable/blob/bf9dd5b2edb9bddda0e317693677b9d95b1e175b/CLAUDE.md
repo: rbrown101010/rilable
kind: claude-md
stars: 109
last_pushed: 2026-06-11T04:22:17Z
license: mit
score: 9
domains: [full-stack, ios-development, agent-orchestration, devops]
tags: [setup-guide, provisioning, end-to-end]
curated: 2026-06-14
curated_by: config-scout
---

# rbrown101010/rilable — claude-md

**Why it's worth keeping:** Uses a 'Things agents commonly get wrong' section for preemptive error correction and provides structured lookup tables for API keys to minimize human intervention.

**Summary:** A masterclass in agent-centric instructions that directs an AI to handle complex, multi-stage environment provisioning and API key management end-to-end.

**Source credibility:** High; specialized full-stack project with active maintenance and clear architectural requirements.

**Recency:** Very current; specifically mentions Xcode 16 and modern toolchains.

**Source:** [rbrown101010/rilable/CLAUDE.md](https://github.com/rbrown101010/rilable/blob/bf9dd5b2edb9bddda0e317693677b9d95b1e175b/CLAUDE.md) · 109★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Rilable — agent setup guide

Rilable is an open-source iOS app that builds **live web apps and native iOS apps from a
prompt** — a Lovable/Replit-mobile-style builder you run on your own accounts. SwiftUI front
end, Convex backend, Claude for code generation, Daytona cloud sandboxes for web apps, Chorus
cloud Xcode builds for iOS apps.

**If you are an AI coding agent (Claude Code etc.): your job is to get this running for the
user end-to-end.** Drive every step below yourself — run the commands, ask the user for keys at
the moments they're needed (with the exact URLs to get them), verify each stage before moving
on, and finish with the app running in the iOS Simulator. The user should never have to read
documentation.

## Architecture (30 seconds)

```
iOS app (SwiftUI, ios/)  ── convex-swift websocket ──►  Convex backend (backend/convex/)
  the user types a prompt          projects/messages/files tables, real-time
                                   "builder" node action orchestrates:
                                   ├─ Anthropic API — Claude writes the app code
                                   ├─ [web]    Daytona REST — public sandbox serves it
```

</details>
