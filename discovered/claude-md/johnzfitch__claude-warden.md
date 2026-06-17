---
name: johnzfitch__claude-warden
source: https://github.com/johnzfitch/claude-warden/blob/cb29f71fd3669f89f6c3571217c9176d7a41cca3/CLAUDE.md
repo: johnzfitch/claude-warden
kind: claude-md
stars: 56
last_pushed: 2026-04-08T09:53:19Z
license: mit
score: 9
domains: [cli-tools, security, observability, agents-ai]
tags: [hooks, monitoring, security-enforcement, otel]
curated: 2026-06-16
curated_by: config-scout
---

# johnzfitch/claude-warden — claude-md

**Why it's worth keeping:** Demonstrates advanced techniques like regex-based field extraction to avoid jq overhead, latency tracking through state files, and sophisticated security filtering (SSRF/RCE prevention).

**Summary:** Provides a comprehensive blueprint for securing and monitoring Claude Code via tool-use lifecycle hooks and an OTEL-compatible observability stack.

**Source credibility:** High; demonstrates deep integration with Claude Code's internal lifecycle events and modern observability standards.

**Recency:** Extremely current; explicitly accounts for recent updates like Elicitation and InstructionsLoaded events.

**Source:** [johnzfitch/claude-warden/CLAUDE.md](https://github.com/johnzfitch/claude-warden/blob/cb29f71fd3669f89f6c3571217c9176d7a41cca3/CLAUDE.md) · 56★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# claude-warden

Token-saving hooks + Go collector backbone for Claude Code observability.

## Repository structure

- `collector/` -- Go service: SQLite store, OTLP receiver (:4319), hook event API (UDS), subagent budget enforcement
- `viewer/` -- htmx web UI for viewing collector data (sessions, tokens, events) on port 8477
- `hooks/` -- Bash hook scripts invoked by Claude Code at tool-use lifecycle events
- `hooks/lib/common.sh` -- Shared library sourced by all hooks (parsing, event emission, latency tracking, sanitization)
- `hooks/lib/otel-trace.sh` -- OTLP/HTTP trace span emitter (bash + curl, fire-and-forget)
- `monitoring/` -- Optional Docker Compose observability stack (Loki, OTEL Collector, Prometheus, Node Exporter, Grafana)
- `monitoring/otel-collector-config.yaml` -- Collector pipelines: logs (otlp + filelog -> Loki), metrics (otlp -> Prometheus), traces (otlp -> debug)
- `monitoring/loki-config.yaml` -- Loki 3.4.2 config (TSDB schema v13, filesystem storage, 30-day retention)
- `monitoring/grafana/` -- Provisioned datasources (Prometheus, Loki) and dashboards
- `tests/` -- Fixture-driven test harness (`bash tests/run.sh`)
- `install.sh` / `uninstall.sh` -- Manages sym
```

</details>
