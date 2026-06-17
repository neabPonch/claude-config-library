---
name: CircleCI-Public__chunk-cli__skill
source: https://github.com/CircleCI-Public/chunk-cli/blob/b5c9daef3d43222553674f200f1290bcc2935e21/skills/chunk-sidecar/SKILL.md
repo: CircleCI-Public/chunk-cli
kind: skill
stars: 81
last_pushed: 2026-06-15T10:49:00Z
license: mit
score: 9
domains: [cli-tools, devops, remote-development]
tags: [sidecar, sync-validate, environment-setup]
curated: 2026-06-15
curated_by: config-scout
---

# CircleCI-Public/chunk-cli — skill

**Why it's worth keeping:** The preflight check pattern (verifying auth/config without leaking secrets) and the highly disciplined setup → snapshot → verify sequence are elite templates for complex tool orchestrations.

**Summary:** This skill manages a remote development loop where local changes are synced to an ephemeral 'sidecar' environment for validation. It provides structured instructions for authentication preflights, creating persistent snapshots of configured environments, and a repeatable sync-validate cycle.

**Source credibility:** High; from an active, specialized developer productivity tool (`chunk-cli`).

**Recency:** Very current; reflects modern ephemeral environment and remote-dev workflows.

**Source:** [CircleCI-Public/chunk-cli/skills/chunk-sidecar/SKILL.md](https://github.com/CircleCI-Public/chunk-cli/blob/b5c9daef3d43222553674f200f1290bcc2935e21/skills/chunk-sidecar/SKILL.md) · 81★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: chunk-sidecar
description: Use when the user says "validate on the sidecar", "run tests on the sidecar", "sync to sidecar", "sidecar dev loop", "check this on the sidecar", "validate remotely", "scaffold test-suites.yml", "set up smarter testing", "write .circleci/test-suites.yml", "run smarter testing doctor", or "diagnose smarter testing", or when you have made edits and want to verify them on a remote `chunk` sidecar instead of running locally. Also covers creating sidecars, snapshotting a configured environment, customizing the sidecar image via `chunk sidecar`, and scaffolding `.circleci/test-suites.yml` for CircleCI Smarter Testing.
version: 1.6.0
allowed-tools:
  - Bash(chunk --version)
  - Bash(chunk auth status)
  - Bash(chunk config set:*)
  - Bash(chunk sidecar:*)
  - Bash(chunk validate:*)
  - Bash(cat .chunk/config.json)
  - Bash(cat .chunk/sidecar.json)
  - Bash(test -n*)
  - Read
  - Write
  - Edit
  - Grep
  - Glob
---

# Chunk Sidecar Skill

Run the user's build, test, and validate commands on a remote `chunk` sidecar instead of locally. The 90% job is the **sync → validate** loop. This skill also covers one-time setup (create, snapshot, environment custo
```

</details>
