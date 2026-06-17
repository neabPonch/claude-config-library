---
name: jahi-suite__tythe-time-tracker
source: https://github.com/jahi-suite/tythe-time-tracker/blob/a1cfc95f5bad07b23fc8458269c2352ffeade433/claude.md
repo: jahi-suite/tythe-time-tracker
kind: claude-md
stars: 0
last_pushed: 2026-02-27T00:23:09Z
license: unknown
score: 8
domains: [agents-ai, workflow-automation]
tags: [agentic-loop, prompt-splitting, task-queue]
curated: 2026-06-14
curated_by: config-scout
---

# jahi-suite/tythe-time-tracker — claude-md

**Why it's worth keeping:** Demonstrates 'prompt splitting' (separate plan/build prompts) and uses an external markdown file as a persistent task queue for state management.

**Summary:** Implements a structured agentic loop using shell scripts and specialized prompt files to separate planning from execution.

**Source credibility:** Low visibility/stars, but the architectural pattern is highly sophisticated and intentional.

**Recency:** Very current; aligns with modern trends in agentic workflow automation.

**Source:** [jahi-suite/tythe-time-tracker/claude.md](https://github.com/jahi-suite/tythe-time-tracker/blob/a1cfc95f5bad07b23fc8458269c2352ffeade433/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code — Tythe Time Tracker

## Structure

```
project-root/
├── loop.sh              # Ralph Wiggum loop runner
├── PROMPT_plan.md       # Planning prompt (./loop.sh plan)
├── PROMPT_build.md      # Build prompt  (./loop.sh)
├── AGENTS.md            # Agent guide: commands, architecture, business rules
├── IMPLEMENTATION_PLAN.md  # Current task queue (populated by ./loop.sh plan)
├── specs/               # Domain requirement specs
│   ├── auth.md
│   ├── time-entries.md
│   ├── exports.md
│   ├── venues.md
│   ├── email-verification.md
│   ├── pay-rates.md
│   └── manager-dashboard.md
├── src/                 # TypeScript/React app (Vite + Express)
├── tythe_time_tracker/  # Python/Streamlit app (legacy reference)
├── scripts/             # Operational utilities
│   ├── install-claude.sh
│   ├── setup-gemini-auth.sh
│   ├── set-cloudrun-env-from-dotenv.sh
│   ├── check-models.sh
│   └── status.sh
└── docs/
    ├── archive/         # Completed historical task records
    └── ...              # Architecture docs, guides
```

## How to run

```bash
# Plan: analyse codebase, update IMPLEMENTATION_PLAN.md
./loop.sh plan

# Build: execute next task from IMPLEMENTATION_PLAN.md
./l
```

</details>
