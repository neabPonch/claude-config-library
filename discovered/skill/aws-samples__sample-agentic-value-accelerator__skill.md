---
name: aws-samples__sample-agentic-value-accelerator__skill
source: https://github.com/aws-samples/sample-agentic-value-accelerator/blob/2a5b4c25bbb432e2e98837ac3ad7079814083258/platform/control_plane/service_approval/plugin/.claude-plugin/skills/generate-iac/SKILL.md
repo: aws-samples/sample-agentic-value-accelerator
kind: skill
stars: 28
last_pushed: 2026-06-14T10:26:00Z
license: apache-2.0
score: 9
domains: [infrastructure-as-code, cloud-security, devops, automation]
tags: [aws, iac, compliance, terraform, cdk]
curated: 2026-06-15
curated_by: config-scout
---

# aws-samples/sample-agentic-value-accelerator — skill

**Why it's worth keeping:** The pattern of including explicit prerequisite filesystem checks, standardized metadata headers, and 'cross-generator consistency' logic is an elite way to handle complex, multi-step agentic workflows. It provides the agent with a mental model for how to verify its own output against external business constraints.

**Summary:** A highly sophisticated skill for generating multi-format (Terraform, CDK, CFN) IaC templates that are strictly compliant with a control matrix. It enforces rigorous cross-generator consistency and automated verification against guard rules.

**Source credibility:** High; developed as part of an official AWS sample for high-compliance financial services environments.

**Recency:** Current; utilizes modern IaC practices and specific validation tools like cfn-guard.

**Source:** [aws-samples/sample-agentic-value-accelerator/platform/control_plane/service_approval/plugin/.claude-plugin/skills/generate-iac/SKILL.md](https://github.com/aws-samples/sample-agentic-value-accelerator/blob/2a5b4c25bbb432e2e98837ac3ad7079814083258/platform/control_plane/service_approval/plugin/.claude-plugin/skills/generate-iac/SKILL.md) · 28★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: generate-iac
description: Generate compliant IaC templates in all 4 formats — modular Terraform, CDK TypeScript, CloudFormation YAML, and CDK for Terraform. Uses parameter coverage matrix from mapping-results.json and API surface from validated.json.
disable-model-invocation: false
argument-hint: '[--service=<name>] [--include-unverified]'
---

# Service Approval — Generator: IaC Templates

Generate compliant infrastructure-as-code templates in all 4 required formats from the
Controls Matrix. Each template implements ALL controls as properties/variables on the
compliant resource.

**Output:** `.service-approval/<slug>/05-generate/iac/`

This is one of 3 focused generate sub-skills. Each writes to separate directories.

---

## Prerequisites

```bash
test -f .service-approval/<slug>/04-map/mapping-results.json && echo "mapping-results: OK" || echo "ERROR"
test -f .service-approval/<slug>/03-validate/validated.json && echo "validated: OK" || echo "ERROR"
```

Create directory structure:
```bash
mkdir -p .service-approval/<slug>/05-generate/iac/modules/_shared
for asset in $(python3 -c "import json; d=json.load(open('.service-approval/<slug>/03-validate/validated.json')); [p
```

</details>
