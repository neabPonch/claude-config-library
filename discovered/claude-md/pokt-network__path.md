---
name: pokt-network__path
source: https://github.com/pokt-network/path/blob/494fd4b8cb99acc75d10461ce88ab85931ff5802/CLAUDE.md
repo: pokt-network/path
kind: claude-md
stars: 12
last_pushed: 2026-06-15T10:44:00Z
license: mit
score: 9
domains: [backend-api, infrastructure, go]
tags: [architectural-mapping, operational-examples, command-reference]
curated: 2026-06-16
curated_by: config-scout
---

# pokt-network/path — claude-md

**Why it's worth keeping:** The 'API Usage' section includes exact curl commands with critical headers, allowing Claude to perform complex operational testing. The component-based architecture breakdown provides a necessary mental model for navigating the Go package structure.

**Summary:** Provides a complete technical blueprint including build commands, architectural hierarchy, and highly specific API interaction patterns.

**Source credibility:** High; active open-source repository from an established decentralized network.

**Recency:** Current; aligns perfectly with modern developer workflows involving Tilt/Kubernetes and CLI-driven prototyping.

**Source:** [pokt-network/path/CLAUDE.md](https://github.com/pokt-network/path/blob/494fd4b8cb99acc75d10461ce88ab85931ff5802/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PATH (Path API & Toolkit Harness) is an open-source Go framework for enabling access to a decentralized supply network. It serves as a gateway that handles service requests and relays them through the Shannon protocol to blockchain endpoints.

## Development Commands

### Building and Running

- `make path_build` - Build the PATH binary locally
- `make path_run` - Run PATH as a standalone binary (requires CONFIG_PATH)
- `make path_up` - Start local Tilt development environment with dependencies
- `make path_down` - Tear down local Tilt development environment

### Testing

- `make test_unit` - Run all unit tests (`go test ./... -short -count=1`)
- `make test_all` - Run unit tests plus E2E tests for key services
- `make e2e_test SERVICE_IDS` - Run E2E tests for specific Shannon service IDs (e.g., `make e2e_test eth,poly`)
- `make load_test SERVICE_IDS` - Run Shannon load tests
- `make go_lint` - Run Go linters (`golangci-lint run --timeout 5m --build-tags test`)

### Configuration

- `make config_prepare_shannon_e2e` - Prepare Shannon E2E configur
```

</details>
