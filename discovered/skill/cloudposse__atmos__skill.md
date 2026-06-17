---
name: cloudposse__atmos__skill
source: https://github.com/cloudposse/atmos/blob/7fc9c3ed55344a94ebb4e9c35952a7b7709d6f73/agent-skills/skills/atmos-validation/SKILL.md
repo: cloudposse/atmos
kind: skill
stars: 1310
last_pushed: 2026-06-15T02:21:55Z
license: apache-2.0
score: 8
domains: [devops, infrastructure-as-code, security]
tags: [terraform, validation, opa, json-schema]
curated: 2026-06-15
curated_by: config-scout
---

# cloudposse/atmos — skill

**Why it's worth keeping:** Provides concrete templates for JSON schemas and Rego policies that allow an agent to validate its own generated configurations against business rules.

**Summary:** Defines a multi-layered validation framework using JSON Schema and OPA/Rego to enforce configuration integrity before Terraform execution.

**Source credibility:** High; Cloud Posse is a highly-regarded entity in the DevOps and Terraform ecosystem.

**Recency:** Current; utilizes modern standards like JSON Schema 2020-12.

**Source:** [cloudposse/atmos/agent-skills/skills/atmos-validation/SKILL.md](https://github.com/cloudposse/atmos/blob/7fc9c3ed55344a94ebb4e9c35952a7b7709d6f73/agent-skills/skills/atmos-validation/SKILL.md) · 1310★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: atmos-validation
description: "Policy validation: OPA/Rego policies, JSON Schema, schema manifests"
metadata:
  copyright: Copyright Cloud Posse, LLC 2026
  version: "1.0.0"
---

# Atmos Validation Framework

## Overview

Atmos provides a built-in validation framework that enforces policies and schema constraints on stack
configurations before infrastructure is provisioned. Validation ensures clean, correct, and compliant
configurations across teams and environments. Atmos supports three types of native validation:

1. **JSON Schema** -- Validates the structure and types of component configurations
2. **Open Policy Agent (OPA)** -- Enforces custom business rules using Rego policies
3. **EditorConfig Checker** -- Ensures consistent coding styles across files

Validation runs automatically before `atmos terraform plan` and `atmos terraform apply`, preventing
misconfigured infrastructure from being provisioned. It can also run on-demand using the
`atmos validate component` and `atmos validate stacks` commands.

## Validation Commands

### `atmos validate component`

Validates a specific component in a stack against configured validation rules:

```shell
# Validate using rule
```

</details>
