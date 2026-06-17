---
name: Nerfherder16__BrickLayer__claude-2026-04-03t03-53-26
source: https://github.com/Nerfherder16/BrickLayer/blob/0bc5157774a31ce90122e13167dc363b98ba8d5f/.claude/CLAUDE.md/CLAUDE.md.2026-04-03T03-53-26
repo: Nerfherder16/BrickLayer
kind: claude-md
stars: 0
last_pushed: 2026-05-04T19:21:43Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, automation]
tags: [orchestration, multi-agent, state-management, agentic-workflows]
curated: 2026-06-16
curated_by: config-scout
---

# Nerfherder16/BrickLayer — claude-md

**Why it's worth keeping:** It demonstrates advanced 'state protection' rules to prevent session corruption and utilizes highly structured agent/skill tables to manage complex task routing.

**Summary:** This config defines a sophisticated multi-agent orchestration layer that treats Claude Code as the interface for a larger research and development framework.

**Source credibility:** Niche experimental project; high complexity suggests a sophisticated individual developer rather than a generic tutorial.

**Recency:** Extremely current, updated within the last month.

**Source:** [Nerfherder16/BrickLayer/.claude/CLAUDE.md/CLAUDE.md.2026-04-03T03-53-26](https://github.com/Nerfherder16/BrickLayer/blob/0bc5157774a31ce90122e13167dc363b98ba8d5f/.claude/CLAUDE.md/CLAUDE.md.2026-04-03T03-53-26) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Standing Rules — Read First

## Never Modify State Files Without Explicit Permission

The following files may be owned by another active Claude session (overnight runs, campaigns, long-running builds). **Never read-then-modify these files unless Tim explicitly asks:**

- `masonry-state.json` — session token, campaign state, Mortar ownership
- `masonry/masonry-state.json` — same
- `.autopilot/mode`, `.autopilot/progress.json`, `.autopilot/compact-state.json`
- `.ui/mode`, `.ui/progress.json`
- `questions.md`, `findings/` (campaign files)

If a value in one of these files looks wrong or inconsistent, **say so and ask** — do not fix it. It may be intentional (future timestamps, future-dated tokens, unusual flags).

---

# BrickLayer + Masonry + Mortar — Architecture

## The Three-Layer Model

```
Claude Code
     ↕
  Masonry          ← the device/bridge (MCP server, hooks, routing engine, schemas)
     ↕
 BrickLayer        ← the layer alongside Claude Code (research loop, campaigns, sims, agent fleet)
```

**BrickLayer** lives alongside Claude Code. It is the full framework: research campaigns, simulations, agent fleet, findings, synthesis. It is NOT a subprocess — it's a parallel l
```

</details>
