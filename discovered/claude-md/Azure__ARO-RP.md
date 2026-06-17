---
name: Azure__ARO-RP
source: https://github.com/Azure/ARO-RP/blob/061c85ae1206c876d536b41002fbaec8d5fafbca/CLAUDE.md
repo: Azure/ARO-RP
kind: claude-md
stars: 119
last_pushed: 2026-06-15T06:25:14Z
license: apache-2.0
score: 9
domains: [backend-api, cloud-infrastructure, go]
tags: [architecture-invariants, safety-rails, multi-module, design-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# Azure/ARO-RP — claude-md

**Why it's worth keeping:** The 'Safety Rails' table mapping sensitive files to documentation guides is elite; the 'Definition of Done' and explicit runtime context maps are highly transferable techniques.

**Summary:** This file provides high-stakes architectural invariants, critical multi-module Go instructions, and specific coding patterns to prevent breaking sensitive systems.

**Source credibility:** High: It is a production-grade configuration from an official Azure resource provider repository.

**Recency:** Highly current, with activity reported within the last month.

**Source:** [Azure/ARO-RP/CLAUDE.md](https://github.com/Azure/ARO-RP/blob/061c85ae1206c876d536b41002fbaec8d5fafbca/CLAUDE.md) · 119★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Azure Red Hat OpenShift RP — ARM resource provider for OpenShift clusters on Azure. Single `aro` binary, multiple modes: rp, monitor, portal, gateway, operator, deploy, mirror, mimo-actuator.

## Architecture Invariant

Cluster mutations (PUT/DELETE) are **async**: Frontend writes to CosmosDB with non-terminal state → Backend polls and processes → updates with terminal state. Never bypass this: frontend handlers must NOT perform cluster operations directly.

## Two Go Modules (critical)

| Module | Path | `go.mod` |
|--------|------|----------|
| Root | `github.com/Azure/ARO-RP` | `go.mod` |
| API | `github.com/Azure/ARO-RP/pkg/api` | `pkg/api/go.mod` |

Root imports API via `replace` directive. **`./...` from root excludes `pkg/api/` tests.** `make unit-test-go` only tests root. To test API: `cd pkg/api && go test ./...`.

> Read `docs/agent-guides/multi-module-build.md` when changing build, test, or formatting targets.

## Essential Commands

```bash
make fmt                 # Format BOTH modules (golangci-lint, NOT gofmt)
make unit-test-go        # Unit tests (root module only)
make lint-go             # Lint
make generate            # Code generation (go generate,
```

</details>
