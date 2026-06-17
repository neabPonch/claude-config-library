---
name: logseq__logseq__skill
source: https://github.com/logseq/logseq/blob/80aeb07d1c0783578e234450e82414d7d3b4bb60/.agents/skills/logseq-repl/SKILL.md
repo: logseq/logseq
kind: skill
stars: 43389
last_pushed: 2026-06-15T04:14:07Z
license: agpl-3.0
score: 9
domains: [cli-tools, development-workflow, devops]
tags: [repl, electron, orchestration, debugging]
curated: 2026-06-15
curated_by: config-scout
---

# logseq/logseq — skill

**Why it's worth keeping:** It features a 'Readiness Model' that uses programmatic state-checking (via shadow-cljs) rather than assuming success, which prevents agents from getting stuck in attach loops. The inclusion of explicit cleanup/port audit logic is highly transferable for complex local development environments.

**Summary:** Orchestrates and verifies a multi-process development environment involving Electron, renderer processes, and Node workers. It provides a structured workflow for starting, verifying, and attaching to specific runtimes.

**Source credibility:** High; part of the Logseq repository, a well-maintained and widely used open-source project.

**Recency:** 

**Source:** [logseq/logseq/.agents/skills/logseq-repl/SKILL.md](https://github.com/logseq/logseq/blob/80aeb07d1c0783578e234450e82414d7d3b4bb60/.agents/skills/logseq-repl/SKILL.md) · 43389★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: logseq-repl
description: Start and coordinate Logseq development REPL workflows for the Desktop renderer `:app`, Electron main-process `:electron`, and `:db-worker-node` runtimes through one unified workflow.
---

# Logseq REPL Workflow

Use this skill when the user needs a Logseq development REPL for:

- Desktop renderer `:app`
- Electron main process `:electron`
- `:db-worker-node`
- any combination of those runtimes

The workflow uses one shared state directory: `<repo>/tmp/logseq-repl/`.

## Scripts

Start everything with the default Logseq data root (`$LOGSEQ_CLI_ROOT_DIR` or `~/logseq`):

```bash
<logseq-repl-skill-dir>/scripts/start-repl.sh --repo demo
```

Start everything with an explicit Logseq data root:

```bash
<logseq-repl-skill-dir>/scripts/start-repl.sh --repo demo --root-dir ~/logseq
```

Clean up everything:

```bash
<logseq-repl-skill-dir>/scripts/cleanup-repl.sh
```

Verify all REPL targets after startup:

```bash
<logseq-repl-skill-dir>/scripts/verify-repls.sh
```

`start-repl.sh` starts:

1. shared `pnpm watch`
2. Desktop dev app via `pnpm dev-electron-app`
3. `db-worker-node` via `node ./static/db-worker-node.js --repo <name> --root-dir <path> --own
```

</details>
