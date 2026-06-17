---
name: moonrhythm__hime
source: https://github.com/moonrhythm/hime/blob/4a68b90929993f85f51978f658d1e473ea4308c8/CLAUDE.md
repo: moonrhythm/hime
kind: claude-md
stars: 67
last_pushed: 2026-06-10T01:47:57Z
license: mit
score: 9
domains: [backend-api, web-frameworks, go]
tags: [architecture-deep-dive, context-injection, error-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# moonrhythm/hime — claude-md

**Why it's worth keeping:** It documents high-stakes 'tribal knowledge' such as specific panic conditions (missing app/routes) and performance details (sync.Pool usage) that standard API docs omit.

**Summary:** This file provides a deep architectural map of the framework, detailing internal mechanics like context injection patterns, error-as-panic conventions, and template rendering logic.

**Source credibility:** A specialized Go web framework with very recent activity and a respectable star count for its niche.

**Recency:** Highly current, covering modern patterns like HTMX and specific Go version requirements.

**Source:** [moonrhythm/hime/CLAUDE.md](https://github.com/moonrhythm/hime/blob/4a68b90929993f85f51978f658d1e473ea4308c8/CLAUDE.md) · 67★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Hime is a minimalist Go web framework built on top of `net/http`. Its core design principle (see `README.md`): it ships **no router or middleware of its own** so it composes with any `net/http`-compatible router, middleware, or handler. Hime only adds an app container, a request `Context` with response helpers, named routes, globals, and an `html/template`-based view/component system.

The module is `github.com/moonrhythm/hime` and requires **Go 1.25**. It is a library (no `main` package).

## Commands

```bash
go test ./...                       # run all tests
go test -run TestApp ./...          # run a single top-level test
go test -run 'TestApp/Clone' ./...  # run a single subtest (tests use t.Run subtests heavily)
go vet ./...                        # static checks (part of CI)
```

CI (`.github/workflows/test.yaml`) runs `go vet` then `go test ./...` on Go 1.25. Tests rely on fixtures in `testdata/` (templates, YAML configs, `server.crt`/`server.key`). Some tests bind real ports (`:8081`, `:8082`) and `time.Sleep` — they run with `t.Parallel()`.

#
```

</details>
