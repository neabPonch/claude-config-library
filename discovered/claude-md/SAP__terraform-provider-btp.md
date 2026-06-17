---
name: SAP__terraform-provider-btp
source: https://github.com/SAP/terraform-provider-btp/blob/5ac7e1daaa48a2713a2d0ccd87d988686dbe25b0/CLAUDE.md
repo: SAP/terraform-provider-btp
kind: claude-md
stars: 118
last_pushed: 2026-06-10T06:50:34Z
license: apache-2.0
score: 9
domains: [cli-tools, infrastructure-as-code, backend-go]
tags: [terraform, go, sap, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# SAP/terraform-provider-btp — claude-md

**Why it's worth keeping:** The 'CRITICAL' command sequences and the 'Common Pitfalls' section offer high-signal instructions that prevent common errors in complex Go development workflows.

**Summary:** Provides a highly structured blueprint for developing Terraform providers, covering build commands, specific file naming conventions, and architectural patterns.

**Source credibility:** High; it is an official SAP repository with recent activity and strong maintenance history.

**Recency:** Very current; reflects modern Terraform Plugin Framework patterns and contemporary Go tooling.

**Source:** [SAP/terraform-provider-btp/CLAUDE.md](https://github.com/SAP/terraform-provider-btp/blob/5ac7e1daaa48a2713a2d0ccd87d988686dbe25b0/CLAUDE.md) · 118★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the official Terraform Provider for SAP Business Technology Platform (SAP BTP). It uses the HashiCorp Terraform Plugin Framework to expose SAP BTP resources, data sources, list resources, provider functions, and actions.

## Essential Commands

Build and development:
- `make fmt` - Format code with gofmt
- `make fix` - Run go fix to update code to newer Go versions
- `make lint` - Run golangci-lint (must pass before commits)
- `make build` - Compile the provider
- `make install` - Build and install to `$GOBIN` for local Terraform dev override
- `make generate` - Generate documentation from code annotations and templates

**CRITICAL: After every code change, always run in order:**
1. `make lint` - Check for linting issues
2. `make fix` - Apply automatic fixes
3. `make build` - Verify compilation

Testing:
- `make test` - Run unit tests with coverage (tagged tests included)
- `make testacc` - Run acceptance tests (requires `TF_ACC=1`, long-running, needs live BTP credentials)
- `go test -v -run TestResourceSubaccountServiceInstance ./btp/pr
```

</details>
