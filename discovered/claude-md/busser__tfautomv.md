---
name: busser__tfautomv
source: https://github.com/busser/tfautomv/blob/b1a070dd2f4c0db63f894a77461a775ec508d5e1/CLAUDE.md
repo: busser/tfautomv
kind: claude-md
stars: 895
last_pushed: 2026-06-14T13:31:43Z
license: apache-2.0
score: 8
domains: [cli-tools, devops, go]
tags: [architecture-documentation, testing-patterns, workflow-guidance]
curated: 2026-06-14
curated_by: config-scout
---

# busser/tfautomv — claude-md

**Why it's worth keeping:** The inclusion of 'Data Flow' and 'Testing' patterns (like golden files) allows an AI to reason about system integrity rather than just syntax.

**Summary:** Acts as a technical manual that outlines component relationships, data flow logic, and specific testing methodologies.

**Source credibility:** High-quality tool with significant community traction (895 stars) and very recent maintenance.

**Recency:** Current; provides highly actionable context for modern Go development workflows.

**Source:** [busser/tfautomv/CLAUDE.md](https://github.com/busser/tfautomv/blob/b1a070dd2f4c0db63f894a77461a775ec508d5e1/CLAUDE.md) · 895★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and Development Commands

- **Build**: `make build` - Builds the tfautomv binary to `bin/tfautomv`
- **Format**: `make fmt` - Formats Go source code using `go fmt`
- **Vet**: `make vet` - Runs `go vet` for static analysis
- **Unit Tests**: `make test` - Runs unit tests in `pkg/` with coverage
- **E2E Tests**: `make test-e2e` - Runs end-to-end tests in `test/e2e/`
- **Full Test**: `make test test-e2e` - Runs both unit and e2e tests
- **Help**: `make help` - Shows available make targets

## Architecture Overview

tfautomv is a Terraform refactoring tool that automatically generates `moved` blocks and `terraform state mv` commands when resources are moved in code.

### Core Components

1. **Engine** (`pkg/engine/`): Core business logic
   - `Plan`: Represents Terraform plans with resources to create/delete
   - `Resource`: Represents a Terraform resource with flattened attributes
   - `Move`: Represents a resource move between addresses/modules
   - `ResourceComparison`: Compares create/delete pairs to detect moves
   - Rules system for ignoring specific attrib
```

</details>
