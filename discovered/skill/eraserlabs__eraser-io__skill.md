---
name: eraserlabs__eraser-io__skill
source: https://github.com/eraserlabs/eraser-io/blob/30d6f3679f597eeae67bacab5ee733c863686177/skills/terraform-diagrams/SKILL.md
repo: eraserlabs/eraser-io
kind: skill
stars: 25
last_pushed: 2026-04-07T17:20:57Z
license: mit
score: 8
domains: [infrastructure-as-code, devops, visualization]
tags: [terraform, diagrams, api-integration, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# eraserlabs/eraser-io — skill

**Why it's worth keeping:** Demonstrates high-quality tool-use instructions including mandatory header injection, strict response formatting (Markdown/Images), and complex relationship mapping logic.

**Summary:** Automatically converts Terraform HCL code into visual architecture diagrams using the Eraser API. It parses resource dependencies and generates a specific DSL to map infrastructure hierarchies.

**Source credibility:** High; developed by Eraser Labs for a specific functional use case.

**Recency:** Current; utilizes modern curl-based API interaction patterns suitable for Claude Code.

**Source:** [eraserlabs/eraser-io/skills/terraform-diagrams/SKILL.md](https://github.com/eraserlabs/eraser-io/blob/30d6f3679f597eeae67bacab5ee733c863686177/skills/terraform-diagrams/SKILL.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: terraform-diagrams
description: 'Generates architecture diagrams from Terraform code. Use when user has .tf files or asks to visualize Terraform infrastructure.'
license: MIT
compatibility: Requires network access to call Eraser API
allowed-tools: Read Write Bash(curl:*)
metadata:
  version: "1.0.0"
  author: Eraser Labs
  tags: terraform, diagram, infrastructure, aws, azure, gcp, iac, hcl
---

# Terraform Diagram Generator

Generates architecture diagrams directly from Terraform `.tf` files. Specializes in parsing Terraform code and visualizing infrastructure resources, modules, and their relationships.

## When to Use

Activate this skill when:

- User has Terraform files (`.tf`, `.tfvars`) and wants to visualize the infrastructure
- User asks to "diagram my Terraform" or "visualize this infrastructure"
- User mentions Terraform, HCL, or infrastructure-as-code
- User wants to see the architecture of their Terraform-managed resources

## How It Works

This skill generates Terraform-specific diagrams by parsing Terraform code and calling the Eraser API directly:

1. **Parse Terraform Files**: Identify resources, modules, data sources, and variables
2. **Extract Relationsh
```

</details>
