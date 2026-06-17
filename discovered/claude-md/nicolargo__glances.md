---
name: nicolargo__glances
source: https://github.com/nicolargo/glances/blob/92156d069425fbe57326e3bdc268c5bfdf994f62/CLAUDE.md
repo: nicolargo/glances
kind: claude-md
stars: 32833
last_pushed: 2026-06-13T14:48:45Z
license: other
score: 9
domains: [cli-tools, security, web-frontend, systems-programming]
tags: [tech-stack, security-rules, ui-principles, deployment-logic]
curated: 2026-06-15
curated_by: config-scout
---

# nicolargo/glances — claude-md

**Why it's worth keeping:** It includes highly specific 'gotcha' warnings (like Snap confinement issues) and precise UI design principles that a generic LLM would otherwise miss.

**Summary:** Provides deep project-specific technical constraints, security protocols, and architectural guardrails that prevent common implementation errors.

**Source credibility:** High; derived from a majorly starred, actively maintained system monitoring tool.

**Recency:** Current; utilizes modern `@` reference patterns optimized for Claude Code sessions.

**Source:** [nicolargo/glances/CLAUDE.md](https://github.com/nicolargo/glances/blob/92156d069425fbe57326e3bdc268c5bfdf994f62/CLAUDE.md) · 32833★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Glances Maintainer Context

> Auto-loaded by Claude Code at the start of every session.
> Glances-specific context. Global principles (role, refactoring strategy,
> contribution tone, communication, output formats) are in `~/.claude/CLAUDE.md`.

---

## Tech stack

| Layer | Technology |
| --- | --- |
| Backend | Python, psutil, FastAPI (REST API), curses (TUI) |
| Frontend | Vue.js, Bootstrap 5, SCSS |
| Export plugins | InfluxDB, MongoDB, MQTT, DuckDB, and others |
| Infrastructure | GitHub Actions, Helm/Kubernetes, Snap (snapcraft) |
| LLM abstraction | LiteLLM (multi-provider) |
| GPU/NPU monitoring | pynvml, sysfs/debugfs |

---

## Reference docs (use `@` to load on demand)

- **Commands & setup**: `@.claude/docs/commands.md`
- **Architecture**: `@.claude/docs/architecture.md`

---

## Code principles (Glances-specific)

### Exception handling for Snap confinement

Wrap the `open()` call inside `try/except`, not just the `read()`. Snap's strict
confinement blocks host file access at the open stage, not the read stage.

### Kubernetes workloads

Use a **DaemonSet** (one pod per node) for system-level monitoring.
Prefer `SYS_PTRACE` over `privileged: true`.

---
```

</details>
