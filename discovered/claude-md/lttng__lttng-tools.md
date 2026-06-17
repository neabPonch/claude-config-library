---
name: lttng__lttng-tools
source: https://github.com/lttng/lttng-tools/blob/8228a8602559e707e5b984aab95bc65831ceb862/CLAUDE.md
repo: lttng/lttng-tools
kind: claude-md
stars: 346
last_pushed: 2026-06-12T16:01:07Z
license: other
score: 9
domains: [systems-programming, cli-tools, c++]
tags: [architecture, coding-standards, build-system, migration]
curated: 2026-06-15
curated_by: config-scout
---

# lttng/lttng-tools — claude-md

**Why it's worth keeping:** It includes explicit mappings of standard library functions to custom project wrappers (e.g., lttng::make_unique) and precise namespace/class structure requirements.

**Summary:** Provides deep architectural context, build instructions, and rigorous coding standards for a C++11 migration project.

**Source credibility:** High; LTTng is a mature, widely-used Linux tracing framework with active maintenance.

**Recency:** Extremely recent; the repository shows activity within the current month.

**Source:** [lttng/lttng-tools/CLAUDE.md](https://github.com/lttng/lttng-tools/blob/8228a8602559e707e5b984aab95bc65831ceb862/CLAUDE.md) · 346★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!--
SPDX-FileCopyrightText: 2025 Philippe Proulx <pproulx@efficios.com>

SPDX-License-Identifier: CC-BY-SA-4.0
-->

# LTTng-tools project context

## Project overview

LTTng-tools is a set of components for controlling LTTng tracing.

Main components:

- **`lttng-sessiond`**: Core tracing control daemon.

   Manages recording sessions (including domains, channels, and event rules) and triggers.

   Receives commands from clients (through liblttng-ctl) and replies to them (Unix socket).

   Spawns and manages `lttng-consumerd` instances.

   Communicates with the user space and Linux kernel tracers.

   Communicates with one or more `lttng-relayd` instances if needed.

- **`lttng-consumerd`**: Trace data consumption daemon.

  Consumes trace data from ring buffers shared with tracers.

  Writes traces to local files or sends it over the network to an `lttng-relayd` instance.

  Separate instances for Linux kernel tracing and user space tracing.

  Spawned by `lttng-sessiond`.

- **`lttng-relayd`**: Network-based trace relay daemon.

  Receives trace data from `lttng-consumerd` instances and commands from `lttng-sessiond` (TCP).

  Writes remote traces (locally).

  Supports LTTng l
```

</details>
