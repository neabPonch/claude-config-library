---
name: pulumi__pulumi-vsphere__claude
source: https://github.com/pulumi/pulumi-vsphere/blob/bc30ad3b3bc9237d48610384a30e7c5d2f59bde9/.claude/CLAUDE.md
repo: pulumi/pulumi-vsphere
kind: claude-md
stars: 60
last_pushed: 2026-06-15T04:34:46Z
license: apache-2.0
score: 8
domains: [infrastructure-as-code, devops, go]
tags: [make, build-systems, ci-safe, negative-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# pulumi/pulumi-vsphere — claude-md

**Why it's worth keeping:** Exceptional use of negative constraints ('Never...', 'Do not...') and a specific 'Good vs Bad' command pattern section to ensure compatibility with CI environments.

**Summary:** A highly structured guide for building Pulumi providers via Make, emphasizing strict boundaries between provider logic and generated SDKs.

**Source credibility:** High; maintained by Pulumi, a major industry standard for Infrastructure as Code.

**Recency:** 

**Source:** [pulumi/pulumi-vsphere/.claude/CLAUDE.md](https://github.com/pulumi/pulumi-vsphere/blob/bc30ad3b3bc9237d48610384a30e7c5d2f59bde9/.claude/CLAUDE.md) · 60★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Pulumi vsphere Provider

This is a Go-based Pulumi resource provider that bridges the Terraform provider to Pulumi. It generates SDKs for TypeScript/JavaScript, Python, .NET, Go, and Java. The provider uses the Terraform provider as an upstream source via git submodules.

## Build Commands

**Always use `make` targets. Never run custom commands unless explicitly instructed.**

### Primary Targets
- `make build` - Build provider and all SDKs
- `make provider` - Build provider binary
- `make schema` - Generate provider schema
- `make tfgen` - Generate SDKs from schema
- `make upstream` - Initialize upstream submodule

### SDK Targets
- `make build_sdks` - Build all SDK packages
- `make build_nodejs` - Build TypeScript/Node.js SDK
- `make build_python` - Build Python SDK
- `make build_dotnet` - Build .NET SDK
- `make build_go` - Build Go SDK
- `make build_java` - Build Java SDK

### Development Targets
- `make lint_provider` - Lint provider Go code
- `make test_provider` - Run provider unit tests

## Repository Structure

```
provider/             -- Go provider implementation
sdk/                  -- Generated SDKs (never edit directly)
upstream/             -- Terraform provider s
```

</details>
