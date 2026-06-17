---
name: pedestal__pedestal
source: https://github.com/pedestal/pedestal/blob/fbb1f8da83831d7683c8003c3db4dbeaeb1613e1/CLAUDE.md
repo: pedestal/pedestal
kind: claude-md
stars: 2770
last_pushed: 2026-06-12T12:10:10Z
license: unknown
score: 9
domains: [backend-api, clojure]
tags: [architecture-heavy, workflow-focused]
curated: 2026-06-15
curated_by: config-scout
---

# pedestal/pedestal — claude-md

**Why it's worth keeping:** It moves beyond commands to explain the system's mental model (Execution Flow/Context Map), which is critical for an AI to reason about changes.

**Summary:** Provides detailed development workflows and a deep technical breakdown of the interceptor-based architecture.

**Source credibility:** High; Pedestal is a widely used, mature Clojure web framework.

**Recency:** Current; includes specific details on modern API transitions (v0.8.0+).

**Source:** [pedestal/pedestal/CLAUDE.md](https://github.com/pedestal/pedestal/blob/fbb1f8da83831d7683c8003c3db4dbeaeb1613e1/CLAUDE.md) · 2770★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Pedestal is a Clojure web framework that brings simplicity, power, and focus to server-side development. It's built around the interceptor pattern and supports asynchronous request handling, Server-Sent Events, and WebSockets as first-class citizens.

**Requirements:**
- Clojure 1.11 or later
- Java 17+
- Servlet API 5.0

## Development Commands

### Running Tests

From the `tests` subdirectory:
```bash
cd tests
clj -X:test
```

The test suite includes a custom test runner (`io.pedestal.test-runner/test`) to avoid test hangs. Tests require JVM options for attaching and async checking which are configured in `tests/deps.edn`.

**Testing utilities:**
- Use `io.pedestal.connector.test/response-for` to test interceptor chains without starting a server
- The `coerce-request-body` protocol handles String, File, or InputStream request bodies
- Tests use `matcher-combinators` for assertions and `mockfn` for mocking

**Running specific tests:**
```bash
# Run a specific namespace
cd tests
clj -M -e "(require 'io.pedestal.http.route-test) (clojure.test/run-
```

</details>
