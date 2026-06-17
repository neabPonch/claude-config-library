---
name: Nyovelt__status-monitor
source: https://github.com/Nyovelt/status-monitor/blob/93a87f77f9945a4285d3ca9f2fd3f602278751ce/claude.md
repo: Nyovelt/status-monitor
kind: claude-md
stars: 0
last_pushed: 2026-04-24T17:15:05Z
license: unknown
score: 8
domains: [backend-api, system-monitoring, fullstack]
tags: [execution-plan, rust, nextjs, technical-spec]
curated: 2026-06-14
curated_by: config-scout
---

# Nyovelt/status-monitor — claude-md

**Why it's worth keeping:** It provides highly specific operational details—such as exact task intervals (1s vs. 5m) and data debouncing logic—that eliminate ambiguity for an AI agent.

**Summary:** A comprehensive technical specification and execution roadmap for a full-stack monitoring system.

**Source credibility:** Low; the unstarred repository and unknown license suggest a personal or prototype project.

**Recency:** 

**Source:** [Nyovelt/status-monitor/claude.md](https://github.com/Nyovelt/status-monitor/blob/93a87f77f9945a4285d3ca9f2fd3f602278751ce/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Here is the full execution plan for the **Status Monitor**.

---

### Phase 1: Architecture & Data Schema

We will use **SQLite** (via `SQLx`) for simplicity and easy deployment in Docker.

#### Database Tables

1. **`clients`**: Registry of monitored servers.
* `id` (UUID), `hostname`, `token`, `last_seen`, `version` (for update checks).


2. **`metrics`**: The raw data dump (Time-Series).
* `id`, `client_id`, `cpu_usage`, `ram_usage`, `disk_usage`, `inode_usage`, `docker_sz`, `gpu_usage`, `timestamp`.
* *Index:* `(client_id, timestamp)` for fast range queries.


3. **`alert_rules`**: User-defined thresholds.
* `id`, `client_id`, `metric_type` (e.g., 'CPU'), `threshold` (e.g., 90.0), `duration_sec` (e.g., must be >90% for 30s).


4. **`settings`**: Global config.
* `key` (e.g., 'slack_webhook_url'), `value`.



---

### Phase 2: Rust Backend (The Orchestrator)

**Stack:** Axum (Server), SQLx (DB), Tokio (Async), Serde.

#### 1. API Layers

* **HTTP (Ingest):** `POST /api/report`
* Accepts JSON batch from client.
* Validates Bearer Token.
* Inserts into DB.
* **Trigger:** Pushes this new data immediately to connected WebSocket clients.
* **Trigger:** Checks `alert_rules`. If a rule
```

</details>
