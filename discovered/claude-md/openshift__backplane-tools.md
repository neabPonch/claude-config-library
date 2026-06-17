---
name: openshift__backplane-tools
source: https://github.com/openshift/backplane-tools/blob/289db43d04d113b1d9a2f6cb03784a1f934eb46a/CLAUDE.md
repo: openshift/backplane-tools
kind: claude-md
stars: 8
last_pushed: 2026-05-12T15:03:14Z
license: apache-2.0
score: 8
domains: [cli-tools, devops, go]
tags: [cli, go, architecture, extension-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# openshift/backplane-tools — claude-md

**Why it's worth keeping:** The prescriptive 'Adding a New Tool' section is an elite pattern for teaching LLMs how to implement new features within existing interfaces. It also documents critical design decisions like OS/arch aliasing and versioning logic that prevent hallucinated implementations.

**Summary:** Provides a comprehensive technical overview including build commands, project structure, and architectural patterns for tool extension.

**Source credibility:** Maintained by the OpenShift ecosystem, ensuring high engineering standards.

**Recency:** Current; uses modern Go toolchain (1.21+) and standard development workflows.

**Source:** [openshift/backplane-tools/CLAUDE.md](https://github.com/openshift/backplane-tools/blob/289db43d04d113b1d9a2f6cb03784a1f934eb46a/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - backplane-tools

## Overview

OpenShift backplane-tools: a CLI tool manager that installs, removes, and upgrades tools used to interact with OpenShift clusters. Built in Go using the Cobra CLI framework.

## Build Commands

```bash
make all        # Default: vet, fmt, mod, lint, test, build
make build      # Build binaries via goreleaser (linux/darwin, 386/amd64/arm64)
make test       # Run all tests
make lint       # Run golangci-lint (v1.55.0)
make fmt        # Format code with gofmt
make vet        # Run go vet
make mod        # Tidy go.mod
make coverage   # Generate code coverage via hack/codecov.sh
```

## Project Structure

```
cmd/                  # CLI subcommands (install, list, remove, upgrade)
pkg/tools/            # Tool implementations and registry
pkg/tools/base/       # Base types: Default, Github, Mirror
pkg/sources/          # Download sources (GitHub API, Cloud Storage, HTTP, OpenShift mirror)
pkg/utils/            # Utilities (checksum, unarchive, gpg, file ops)
hack/                 # CI scripts (codecov)
main.go               # Entry point (Cobra root command)
```

## Architecture

### Tool Interface (`pkg/tools/tools.go`)

All managed tools impl
```

</details>
