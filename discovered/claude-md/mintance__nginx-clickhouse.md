---
name: mintance__nginx-clickhouse
source: https://github.com/mintance/nginx-clickhouse/blob/f57462c66cbdef207c98d194dad13a975c4cc706/CLAUDE.md
repo: mintance/nginx-clickhouse
kind: claude-md
stars: 159
last_pushed: 2026-05-09T13:01:37Z
license: apache-2.0
score: 9
domains: [backend, data-engineering, go]
tags: [architecture-map, style-guide, testing-rigor]
curated: 2026-06-16
curated_by: config-scout
---

# mintance/nginx-clickhouse — claude-md

**Why it's worth keeping:** The detailed mapping of files to responsibilities and the granular code conventions (e.g., error wrapping and naming rules) are perfect for ensuring AI-generated edits remain idiomatic and consistent.

**Summary:** This file provides a comprehensive architectural blueprint and strict coding standards for a high-performance Go microservice.

**Source credibility:** High; shows professional engineering patterns typical of a well-maintained, starred open-source project.

**Recency:** Very current; references modern Go 1.26 features and contemporary toolchain workflows.

**Source:** [mintance/nginx-clickhouse/CLAUDE.md](https://github.com/mintance/nginx-clickhouse/blob/f57462c66cbdef207c98d194dad13a975c4cc706/CLAUDE.md) · 159★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

nginx-clickhouse is a Go microservice that tails NGINX access logs and batch-inserts parsed entries into ClickHouse using the native TCP protocol. It supports both traditional text log formats and JSON access logs (`log_format escape=json`), and provides log enrichment (auto-hostname, environment, service tags, status class, referrer domain, URL extension, bot detection, browser/OS/device via user-agent parsing). It features retry with exponential backoff, optional disk buffering for crash recovery, circuit breaker, optional server-side batching via ClickHouse async inserts, structured JSON logging, and Prometheus metrics.

## Architecture

```
main.go                    → Entry point: tail, buffer, flush loop, graceful shutdown, /healthz
config/config.go           → YAML config + env var overrides (structured types)
nginx/nginx.go             → Parses NGINX log lines using gonx (configurable log format)
nginx/json.go              → Parses NGINX JSON access logs (log_format escape=json) and applies enrichments
filter/filter.go           → Expression-based filtering and sampling (expr-lang/expr)
clickhouse/clickhouse.go   → Client struct: connection
```

</details>
