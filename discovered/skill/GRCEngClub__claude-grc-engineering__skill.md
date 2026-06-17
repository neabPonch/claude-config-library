---
name: GRCEngClub__claude-grc-engineering__skill
source: https://github.com/GRCEngClub/claude-grc-engineering/blob/42cdc088b73f89431c233aa737004b01e77299c7/plugins/grc-engineer/skills/code-to-control-mapper/SKILL.md
repo: GRCEngClub/claude-grc-engineering
kind: skill
stars: 308
last_pushed: 2026-06-14T08:16:08Z
license: other
score: 8
domains: [devsecops, compliance, security, infrastructure-as-code]
tags: [grc, audit, iaC, security]
curated: 2026-06-16
curated_by: config-scout
---

# GRCEngClub/claude-grc-engineering — skill

**Why it's worth keeping:** Demonstrates how to bridge LLM reasoning with deterministic programmatic analysis through external CLI tools; provides a pattern for generating structured, audit-ready evidence reports.

**Summary:** Maps infrastructure-as-code (IaC) files to compliance frameworks like SOC 2 and ISO 27001 by invoking specialized mapping scripts.

**Source credibility:** High; the repository shows significant community interest with 308 stars and active maintenance.

**Recency:** Current; optimized for modern agentic workflows involving bash/node tool execution.

**Source:** [GRCEngClub/claude-grc-engineering/plugins/grc-engineer/skills/code-to-control-mapper/SKILL.md](https://github.com/GRCEngClub/claude-grc-engineering/blob/42cdc088b73f89431c233aa737004b01e77299c7/plugins/grc-engineer/skills/code-to-control-mapper/SKILL.md) · 308★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-to-control-mapper
description: Maps infrastructure code (Terraform, Kubernetes, CloudFormation) to compliance controls (ISO 27001, SOC 2, NIST 800-53). Analyzes IaC files and generates compliance evidence mappings showing which controls are satisfied.
allowed-tools: Bash, Read, Glob, Write, Edit
---

# Code-to-Control Mapper

Maps infrastructure-as-code (IaC) files to specific compliance framework controls. Translates technical implementations into audit-ready compliance evidence.

## Quick Commands

**Map a Terraform file to SOC 2:**

```bash
node plugins/grc-engineer/scripts/map-control.js main.tf SOC2
```

**Map Kubernetes manifests to ISO 27001:**

```bash
node plugins/grc-engineer/scripts/map-control.js k8s/deployment.yaml ISO27001
```

**Map CloudFormation template to NIST 800-53:**

```bash
node plugins/grc-engineer/scripts/map-control.js template.yaml NIST80053
```

## Supported Frameworks

- **SOC2** - Service Organization Control 2 (CC6.1, CC7.2, etc.)
- **ISO27001** - ISO/IEC 27001 (Annex A controls)
- **NIST80053** - NIST Special Publication 800-53
- **PCIDSS** - Payment Card Industry Data Security Standard
- **HIPAA** - Health Insurance Portability and A
```

</details>
