---
name: mk-knight23__AGENTS-COLLECTION__setup-skill
source: https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/.CLAUDE/setup-SKILL.md
repo: mk-knight23/AGENTS-COLLECTION
kind: skill
stars: 72
last_pushed: 2026-04-16T07:24:00Z
license: unknown
score: 9
domains: [cli-tools, devops, agents-ai, systems-administration]
tags: [setup, orchestration, self-healing, environment-config]
curated: 2026-06-16
curated_by: config-scout
---

# mk-knight23/AGENTS-COLLECTION — skill

**Why it's worth keeping:** Excellent use of self-healing logic, platform-specific branching for macOS/Linux, and highly specific error recovery procedures like the Docker socket permission fix.

**Summary:** An advanced orchestration skill that automates complex environment setup including Node.js versions, container runtimes (Docker vs Apple Container), and messaging channel integrations.

**Source credibility:** The detailed system administration commands suggest a high-quality, purpose-built tool rather than generic AI output.

**Recency:** Very current; references Node 22 and modern containerization workflows.

**Source:** [mk-knight23/AGENTS-COLLECTION/DOCS/.CLAUDE/setup-SKILL.md](https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/.CLAUDE/setup-SKILL.md) · 72★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: setup
description: Run initial NanoClaw setup. Use when user wants to install dependencies, authenticate messaging channels, register their main channel, or start the background services. Triggers on "setup", "install", "configure nanoclaw", or first-time setup requests.
---

# NanoClaw Setup

Run setup steps automatically. Only pause when user action is required (channel authentication, configuration choices). Setup uses `bash setup.sh` for bootstrap, then `npx tsx setup/index.ts --step <name>` for all other steps. Steps emit structured status blocks to stdout. Verbose logs go to `logs/setup.log`.

**Principle:** When something is broken or missing, fix it. Don't tell the user to go fix it themselves unless it genuinely requires their manual action (e.g. authenticating a channel, pasting a secret token). If a dependency is missing, install it. If a service won't start, diagnose and repair. Ask the user for permission when needed, then do the work.

**UX Note:** Use `AskUserQuestion` for all user-facing questions.

## 1. Bootstrap (Node.js + Dependencies)

Run `bash setup.sh` and parse the status block.

- If NODE_OK=false → Node.js is missing or too old. Use `AskUserQues
```

</details>
