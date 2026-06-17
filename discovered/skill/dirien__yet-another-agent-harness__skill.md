---
name: dirien__yet-another-agent-harness__skill
source: https://github.com/dirien/yet-another-agent-harness/blob/5bc3b04124d4d8d7f80cc6974a665b2a47e53639/.claude/skills/pulumi-go/SKILL.md
repo: dirien/yet-another-agent-harness
kind: skill
stars: 19
last_pushed: 2026-05-31T00:33:08Z
license: mit
score: 9
domains: [infrastructure-as-code, devops, golang]
tags: [pulumi, go, iac, esc]
curated: 2026-06-15
curated_by: config-scout
---

# dirien/yet-another-agent-harness — skill

**Why it's worth keeping:** It includes high-value patterns like ComponentResource implementation and structured error recovery workflows which are critical for agentic reliability in IaC.

**Summary:** A comprehensive guide for managing Pulumi Go infrastructure with a heavy focus on advanced Pulumi ESC (Environments, Secrets, Configuration) integration.

**Source credibility:** The source is a specialized Go harness with niche, professional-grade technical content.

**Recency:** Highly current, integrating modern Pulumi ESC orchestration techniques.

**Source:** [dirien/yet-another-agent-harness/.claude/skills/pulumi-go/SKILL.md](https://github.com/dirien/yet-another-agent-harness/blob/5bc3b04124d4d8d7f80cc6974a665b2a47e53639/.claude/skills/pulumi-go/SKILL.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pulumi-go
description: Creates Pulumi infrastructure-as-code projects in Go, configures OIDC authentication, integrates with Pulumi ESC for centralized secrets and configuration management, and builds multi-language component resources. Use when setting up Pulumi Go projects, writing infrastructure code with Go, configuring OIDC for Pulumi, using Pulumi ESC with Go, automating cloud infrastructure with Golang, creating reusable Pulumi components in Go, or working with pulumi-go-provider. Also use when the user mentions Pulumi with Go/Golang, AWS/Azure/GCP infrastructure in Go, or Go-based ComponentResource patterns.
---

# Pulumi Go Skill

## Development Workflow

### 1. Project Setup

```bash
# Create new Go project
pulumi new go

# Or with a cloud-specific template
pulumi new aws-go
pulumi new azure-go
pulumi new gcp-go
```

### 2. Pulumi ESC Integration

**Link ESC environment to stack:**
```bash
# Create ESC environment
pulumi env init myorg/myproject-dev

# Edit environment
pulumi env edit myorg/myproject-dev

# Link to Pulumi stack
pulumi config env add myorg/myproject-dev
```

**ESC environment definition (YAML):**
```yaml
values:
  # Static configuration
  pulumiC
```

</details>
