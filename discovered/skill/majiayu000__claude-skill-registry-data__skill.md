---
name: majiayu000__claude-skill-registry-data__skill
source: https://github.com/majiayu000/claude-skill-registry-data/blob/52f0e3b5880c90b2d53b06e0a6f081bf5a57deba/design/import-pulumi/SKILL.md
repo: majiayu000/claude-skill-registry-data
kind: skill
stars: 10
last_pushed: 2026-06-16T04:50:55Z
license: unknown
score: 9
domains: [devops, infrastructure-as-code, gcp, pulumi]
tags: [import, iac, gcp, automation]
curated: 2026-06-16
curated_by: config-scout
---

# majiayu000/claude-skill-registry-data — skill

**Why it's worth keeping:** The 'Import ID Formats' mapping table is a perfect template for how to handle complex syntax requirements. The execution flow includes critical safety constraints like one-at-a-time imports and mandatory verification steps.

**Summary:** Provides a highly structured workflow for importing existing GCP resources into Pulumi state via CLI.

**Source credibility:** High-quality content structure suggests a practical, real-world DevOps use case.

**Recency:** Highly relevant; Pulumi/GCP workflows are contemporary industry standards.

**Source:** [majiayu000/claude-skill-registry-data/design/import-pulumi/SKILL.md](https://github.com/majiayu000/claude-skill-registry-data/blob/52f0e3b5880c90b2d53b06e0a6f081bf5a57deba/design/import-pulumi/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: import-pulumi
description: Guide for importing existing Google Cloud resources into Pulumi state. Use when the user says "import resource to Pulumi", "add existing GCP resource", or needs to bring existing infrastructure under Pulumi management.
---

# import-pulumi

Import existing GCP resources into Pulumi state.

## Trigger Examples

- "Import resource to Pulumi"
- "Add existing GCP resource to state"
- "Bring this resource under Pulumi management"

## Prerequisites

- Pulumi project exists under `infra/`
- Target resources already exist in Google Cloud
- Pulumi backend (GCS) is configured
- Authentication to Google Cloud is available

## Execution Flow

### 1. Confirm Stack and Resource Type

Validate stack is one of: `shared`, `dev`, `prod`

### 2. Gather Resource Information

Prompt for GCP metadata:

- Project ID (e.g., `koborin-ai`)
- Region/location (`asia-northeast1`)
- Resource name/ID
- Any secondary identifiers

### 3. Resolve Pulumi Resource Name

Inspect `infra/src/stacks/*.ts` to find the Pulumi resource name.

### 4. Build Import Command

Use CLI-based import (NOT code-based import options):

```bash
cd infra
pulumi stack select <stack>
pulumi import <res
```

</details>
