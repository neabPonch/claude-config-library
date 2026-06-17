---
name: alexei-led__pumba
source: https://github.com/alexei-led/pumba/blob/69b78e6d286cc1da33c192df2a591b0335582bd7/CLAUDE.md
repo: alexei-led/pumba
kind: claude-md
stars: 3051
last_pushed: 2026-06-08T03:15:22Z
license: apache-2.0
score: 10
domains: [cli-tools, devops, go]
tags: [build-systems, architecture-guidance, testing-workflows]
curated: 2026-06-14
curated_by: config-scout
---

# alexei-led/pumba — claude-md

**Why it's worth keeping:** It includes strict coding mandates (e.g., 'MUST use this helper', 'Never re-introduce...') and provides specific, environment-aware testing commands for Colima/Podman that are crucial for automated verification.

**Summary:** A gold-standard file that combines exhaustive build/test instructions with deep architectural 'laws' and constraints. It explicitly defines how to extend the system without breaking established patterns.

**Source credibility:** Extremely high; a mature, highly-starred (3k+) industry tool with active maintenance.

**Recency:** Very current, accounting for modern container runtimes like Podman and recent Go ecosystem practices.

**Source:** [alexei-led/pumba/CLAUDE.md](https://github.com/alexei-led/pumba/blob/69b78e6d286cc1da33c192df2a591b0335582bd7/CLAUDE.md) · 3051★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Pumba Development Guide

## Build & Test Commands

- **Build:** `make build` (builds for current TARGETOS/TARGETARCH)
- **Full pipeline:** `make all` (format → lint → test → build)
- **Unit tests:** `make test` (requires `CGO_ENABLED=1` for race detector)
- **Test with coverage:** `make test-coverage`
- **Race detector:** `make test-race` (linux/amd64 only)
- **Lint:** `make lint` (runs golangci-lint with `.golangci.yaml`)
- **Format:** `make fmt`
- **Cross-compile:** `make release` (darwin/linux/windows × amd64/arm64)
- **Integration tests:** `make integration-tests` (requires Docker, uses bats)
- **All integration tests:** `make integration-tests-all` (includes stress tests)
- **Advanced Go integration tests:** `make integration-tests-advanced` (Go-based tests in `tests/integration/`)
- **Generate mocks:** `make mocks` (uses mockery)
- **Unit tests in sandbox:** `CGO_ENABLED=0 go test ./...` (skips race detector, works without CGO toolchain)

## Integration Testing

Integration tests use [bats](https://github.com/bats-core/bats-core):

- Tests are in `tests/*.bats` with helpers in `tests/test_helper.bash`
- **Run all tests locally (recommended):** `colima ssh -- sudo bats tests
```

</details>
