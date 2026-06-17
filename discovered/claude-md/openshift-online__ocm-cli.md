---
name: openshift-online__ocm-cli
source: https://github.com/openshift-online/ocm-cli/blob/14079f029600c65ce50828f6aa6ba8aee98a9ae0/CLAUDE.md
repo: openshift-online/ocm-cli
kind: claude-md
stars: 90
last_pushed: 2026-06-11T15:00:36Z
license: apache-2.0
score: 8
domains: [cli-tools, backend, go]
tags: [architecture-mapping, command-reference, go-lang]
curated: 2026-06-15
curated_by: config-scout
---

# openshift-online/ocm-cli — claude-md

**Why it's worth keeping:** It maps specific package directories to their functional responsibilities, which prevents the AI from wandering during discovery. It also explicitly defines technical patterns like connection management and output formatting.

**Summary:** Provides a comprehensive structural map and essential development workflows for a complex Go-based CLI.

**Source credibility:** High; comes from an active Red Hat OpenShift project with very recent updates.

**Recency:** Current; reflects modern Go development standards and container-native workflows.

**Source:** [openshift-online/ocm-cli/CLAUDE.md](https://github.com/openshift-online/ocm-cli/blob/14079f029600c65ce50828f6aa6ba8aee98a9ae0/CLAUDE.md) · 90★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

OCM CLI is a command-line tool for interacting with the OpenShift Cluster Manager (OCM) API at api.openshift.com. The codebase is a Go application built around Cobra for command structure and the OCM SDK for API interactions.

## Development Commands

### Building
- `make` or `make cmds` - Build all command binaries
- `make install` - Install the `ocm` binary to Go's bin directory
- `go build "./cmd/ocm"` - Build just the main ocm binary

### Testing
- `make test` or `make tests` - Run all tests using Ginkgo
- `make ginkgo-install` - Install Ginkgo test framework locally
- Tests are located in the `tests/` directory and use Ginkgo/Gomega

### Code Quality
- `make lint` - Run golangci-lint using podman/docker container (version defined in `.golangciversion`)
- `make fmt` - Format Go code using gofmt
- `make clean` - Clean build artifacts

### Container Support
- Use `podman` instead of `docker` (configurable via `container_runner` variable)
- `make build_release_images` - Build release container images

## Architecture

### Command Structure
The CLI uses
```

</details>
