---
name: sw-embed__cor24-rs
source: https://github.com/sw-embed/cor24-rs/blob/40033d90e80dcef1a420bd3db7c8fd22fb9f181f/CLAUDE.md
repo: sw-embed/cor24-rs
kind: claude-md
stars: 0
last_pushed: 2026-05-03T21:09:31Z
license: mit
score: 9
domains: [rust, webassembly, agents-ai, embedded-systems]
tags: [session-protocol, build-automation, workflow-enforcement]
curated: 2026-06-15
curated_by: config-scout
---

# sw-embed/cor24-rs — claude-md

**Why it's worth keeping:** It demonstrates how to enforce a ritualistic session lifecycle (start -> work -> complete -> stop) and uses 'CRITICAL' warnings to steer the AI away from raw commands that break the environment.

**Summary:** Defines a strict state machine for agent sessions and provides high-precision build/deployment instructions to prevent common tool errors.

**Source credibility:** Low star count, but the extreme technical density suggests highly specialized domain expertise.

**Recency:** Very recent; updated within the last month.

**Source:** [sw-embed/cor24-rs/CLAUDE.md](https://github.com/sw-embed/cor24-rs/blob/40033d90e80dcef1a420bd3db7c8fd22fb9f181f/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## CRITICAL: AgentRail Session Protocol (MUST follow exactly)

This project uses AgentRail. Every session follows this exact sequence:

### 1. START (do this FIRST, before anything else)
```bash
agentrail next
```
Read the output carefully. It tells you your current step, prompt, skill docs, and past trajectories.

### 2. BEGIN (immediately after reading the next output)
```bash
agentrail begin
```

### 3. WORK (do what the step prompt says)
Do NOT ask the user "want me to proceed?" or "shall I start?". The step prompt IS your instruction. Execute it.

### 4. COMMIT (after the work is done)
Commit your code changes with git.

### 5. COMPLETE (LAST thing, after committing)
```bash
agentrail complete --summary "what you accomplished" \
  --reward 1 \
  --actions "tools and approach used" \
  --next-slug "next-step-slug" \
  --next-prompt "what the next step should do" \
  --next-task-type "task-type"
```
If the step failed: `--reward -1 --failure-mode "what went wrong"`
If the saga is finished: add `--done`

### 6. STOP (after complete, DO NOT continue working)
Do NOT
```

</details>
